# Приемы для повышения чистоты кода PHP

### Делать отступы как можно меньше

До

    class DiscountApplier
    {
        private DiscountCalculator $calculator;

        public function __construct(DiscountCalculator $calculator)
        {
            $this->calculator = $calculator;
        }

        public function apply(Basket $basket): void
        {
            if ($basket->hasItems()) {
                $discount = 0.0;

                foreach ($basket->getItems() as $basketItem) {
                    if ($basketItem->isTaxable()) {
                        if ($basketItem->getPrice() > 0) {
                            $discount += $this->calculator->getDiscount($basketItem);
                        }
                    }
                }

                $basket->applyDiscount($discount);
            }
        }
    }

После

    class DiscountApplier
    {
        private DiscountCalculator $calculator;

        public function __construct(DiscountCalculator $calculator)
        {
            $this->calculator = $calculator;
        }

        public function apply(Basket $basket): void
        {
            if (!$basket->hasItems()) {
                return;
            }

            $discount = 0.0;

            foreach ($this->getDiscountableItems($basket) as $basketItem) {
                $discount += $this->calculator->getDiscount($basketItem);
            }

            $basket->applyDiscount($discount);
        }

        /**
         * @return iterable<BasketItem>
         */
        private function getDiscountableItems(Basket $basket): iterable
        {   
            foreach ($basket->getItems() as $basketItem) {
                if (!$basketItem->isTaxable() || $basketItem->getPrice() === 0) {
                    continue;
                }

                yield $basketItem;
            }
        }
    }
