# Приемы для повышения чистоты кода PHP

---

[Делать отступы как можно меньше](https://github.com/neurohotep/phptricks#%D0%B4%D0%B5%D0%BB%D0%B0%D1%82%D1%8C-%D0%BE%D1%82%D1%81%D1%82%D1%83%D0%BF%D1%8B-%D0%BA%D0%B0%D0%BA-%D0%BC%D0%BE%D0%B6%D0%BD%D0%BE-%D0%BC%D0%B5%D0%BD%D1%8C%D1%88%D0%B5)

---

### Старайтесть делать отступы как можно меньше

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


### Удаляйте ненужные блоки в условиях

До 

    function mapOrderStatusToLabel(Order $order): string
    {
        if ($order->isComplete()) {
            return 'Completed';
        } elseif ($order->isPending()) {
            return 'In transport';
        } else {
            return 'New';
        }
    }

После

    function mapOrderStatusToLabel(Order $order): string
    {
        if ($order->isComplete()) {
            return 'Completed';
        }

        if ($order->isPending()) {
            return 'In transport';
        }

        return 'New';
    }
