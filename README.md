# Приемы для повышения чистоты кода PHP

### Делать отступы как можно меньше

    <?php

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
