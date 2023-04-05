# Приемы для повышения чистоты кода PHP

---

* [Старайтесь делать отступы как можно меньше](https://github.com/neurohotep/phptricks/blob/main/README.md#%D1%81%D1%82%D0%B0%D1%80%D0%B0%D0%B9%D1%82%D0%B5%D1%81%D1%82%D1%8C-%D0%B4%D0%B5%D0%BB%D0%B0%D1%82%D1%8C-%D0%BE%D1%82%D1%81%D1%82%D1%83%D0%BF%D1%8B-%D0%BA%D0%B0%D0%BA-%D0%BC%D0%BE%D0%B6%D0%BD%D0%BE-%D0%BC%D0%B5%D0%BD%D1%8C%D1%88%D0%B5)
* [Удаляйте ненужные блоки в условиях](https://github.com/neurohotep/phptricks/blob/main/README.md#%D1%83%D0%B4%D0%B0%D0%BB%D1%8F%D0%B9%D1%82%D0%B5-%D0%BD%D0%B5%D0%BD%D1%83%D0%B6%D0%BD%D1%8B%D0%B5-%D0%B1%D0%BB%D0%BE%D0%BA%D0%B8-%D0%B2-%D1%83%D1%81%D0%BB%D0%BE%D0%B2%D0%B8%D1%8F%D1%85)
* [Меняйте местами условия, чтобы уменьшить отступы](https://github.com/neurohotep/phptricks/blob/main/README.md#%D0%BC%D0%B5%D0%BD%D1%8F%D0%B9%D1%82%D0%B5-%D0%BC%D0%B5%D1%81%D1%82%D0%B0%D0%BC%D0%B8-%D1%83%D1%81%D0%BB%D0%BE%D0%B2%D0%B8%D1%8F-%D1%87%D1%82%D0%BE%D0%B1%D1%8B-%D1%83%D0%BC%D0%B5%D0%BD%D1%8C%D1%88%D0%B8%D1%82%D1%8C-%D0%BE%D1%82%D1%81%D1%82%D1%83%D0%BF%D1%8B)
* [Используйте switch вместо if там, где это возможно](https://github.com/neurohotep/phptricks/blob/main/README.md#%D0%B8%D1%81%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D1%83%D0%B9%D1%82%D0%B5-switch-%D0%B2%D0%BC%D0%B5%D1%81%D1%82%D0%BE-if-%D1%82%D0%B0%D0%BC-%D0%B3%D0%B4%D0%B5-%D1%8D%D1%82%D0%BE-%D0%B2%D0%BE%D0%B7%D0%BC%D0%BE%D0%B6%D0%BD%D0%BE)
* [Разбивайте сложные уравнения для краткости](https://github.com/neurohotep/phptricks/blob/main/README.md#%D1%80%D0%B0%D0%B7%D0%B1%D0%B8%D0%B2%D0%B0%D1%82%D1%8C-%D1%81%D0%BB%D0%BE%D0%B6%D0%BD%D1%8B%D0%B5-%D1%83%D1%80%D0%B0%D0%B2%D0%BD%D0%B5%D0%BD%D0%B8%D1%8F-%D0%B4%D0%BB%D1%8F-%D0%BA%D1%80%D0%B0%D1%82%D0%BA%D0%BE%D1%81%D1%82%D0%B8)
* [Расставляйте условия в логическом порядке в операторах if](https://github.com/neurohotep/phptricks/blob/main/README.md#%D1%80%D0%B0%D1%81%D1%81%D1%82%D0%B0%D0%B2%D0%BB%D1%8F%D1%82%D1%8C-%D1%83%D1%81%D0%BB%D0%BE%D0%B2%D0%B8%D1%8F-%D0%B2-%D0%BB%D0%BE%D0%B3%D0%B8%D1%87%D0%B5%D1%81%D0%BA%D0%BE%D0%BC-%D0%BF%D0%BE%D1%80%D1%8F%D0%B4%D0%BA%D0%B5-%D0%B2-%D0%BE%D0%BF%D0%B5%D1%80%D0%B0%D1%82%D0%BE%D1%80%D0%B0%D1%85-if)
* [Предпочитайте именованные методы флагам](https://github.com/neurohotep/phptricks/blob/main/README.md#%D0%BF%D1%80%D0%B5%D0%B4%D0%BF%D0%BE%D1%87%D0%B8%D1%82%D0%B0%D0%B9%D1%82%D0%B5-%D0%B8%D0%BC%D0%B5%D0%BD%D0%BE%D0%B2%D0%B0%D0%BD%D0%BD%D1%8B%D0%B5-%D0%BC%D0%B5%D1%82%D0%BE%D0%B4%D1%8B-%D1%84%D0%BB%D0%B0%D0%B3%D0%B0%D0%BC)
* [Используйте деструктуризацию массива](https://github.com/neurohotep/phptricks/blob/main/README.md#%D0%B8%D1%81%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D1%83%D0%B9%D1%82%D0%B5-%D0%B4%D0%B5%D1%81%D1%82%D1%80%D1%83%D0%BA%D1%82%D1%83%D1%80%D0%B8%D0%B7%D0%B0%D1%86%D0%B8%D1%8E-%D0%BC%D0%B0%D1%81%D1%81%D0%B8%D0%B2%D0%B0)
* [array_column для маппинга данных](https://github.com/neurohotep/phptricks/blob/main/README.md#array_column-%D0%B4%D0%BB%D1%8F-%D0%BC%D0%B0%D0%BF%D0%BF%D0%B8%D0%BD%D0%B3%D0%B0-%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85)

---

### Старайтесь делать отступы как можно меньше

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

---

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

---

### Меняйте местами условия, чтобы уменьшить отступы

До

    function act(bool $success)
    {
        if ($success) {
            // towering block of code
            // towering block of code
            // towering block of code
            // towering block of code
            // towering block of code
            // towering block of code
            // towering block of code
        } else {
            // one liner
        }
    }
    
После

    function act(bool $success)
    {
        if (!$success) {
            // one liner
            return;
        }

        // towering block of code
        // towering block of code
        // towering block of code
        // towering block of code
        // towering block of code
        // towering block of code
        // towering block of code
    }

---

### Используйте switch вместо if там, где это возможно

До

    function mapOrderStatusToLabel(Order $order): string
    {
        $label = 'unknown';

        if ('complete' === $order->getStatus()) {
            $label = 'Completed';
        }

        if ('pending' === $order->getStatus()) {
            $label = 'In transport';
        }

        if ('new' === $order->getStatus()) {
            $label = 'New';
        }

        return $label';
    }
    
После

    function mapOrderStatusToLabel(Order $order): string
    {
        switch ($order->getStatus()) {
            case 'complete':
                return 'Completed';

            case 'pending':
            case 'in_transport':
                return 'In transport';

            case 'new':
                return 'New';

            default:
                return 'unknown';
        }
    }
    
---

### Разбивать сложные уравнения для краткости

До

    function getTotalWithTax(Payment $payment, int $taxPercent): float
    {
        // is the order correct at all?

        return (float) (int) $payment->getTotal() * (1 + $taxPercent / 100);
    }
    
После

    function getTotalWithTax(Payment $payment, int $taxPercent): float
    {
        // descriptive variables with intermediary values for easier debugging
        $paymentAmount = (int) $payment->getAmount();
        $taxCoefficient = 1 + ($taxPercent / 100);

        $totalWithTax = $paymentAmount * $taxCoefficient;

        return (float) $totalWithTax;
    }
    
---

### Расставлять условия в логическом порядке в операторах if

До

    if ($httpApi->hasAccess($user) && $user->isActive() && $isSuccess) {
        // all conditions must be met in order for this condition to execute
        // in case of 'and' we should keep the heaviest conditions last
        // and the fastest to execute in front
    }
    
После

    if ($isSuccess && $user->isActive() && $httpApi->hasAccess($user)) {
        // if $isSuccess is false
        // other conditions will not be evaluated
    }
    
---

### Предпочитайте именованные методы флагам

До

    class UserRepository
    {
        public function getUsers(?bool $includingDeleted = false): array
        {
        }
    }
    
После

    class UserRepository
    {
        public function getUsers(): array
        {
        }

        public function getUsersIncludingDeleted(): array
        {
        }
    }
    
---

### Используйте деструктуризацию массива

До

    $workers = [
      ['id' => 1, 'name' => 'John Doe'],
      ['id' => 3, 'name' => 'Jane Doe'],
      ['id' => 4, 'name' => 'Monica Trullo'],
      ['id' => 5, 'name' => 'Jonathan Bank'],
    ];

    foreach ($workers as $worker) {
      $workerId = $worker['id'];
      $workerName = $worker['name'];

      // …
    }
    
После

    $workers = [
      ['id' => 1, 'name' => 'John Doe'],
      ['id' => 3, 'name' => 'Jane Doe'],
      ['id' => 4, 'name' => 'Monica Trullo'],
      ['id' => 5, 'name' => 'Jonathan Bank'],
    ];

    foreach ($workers as ['id' => $workerId, 'name' => $workerName]) {
      // …
    }
    
---

### array_column для маппинга данных

До

    $userAvatars = [];
    foreach ($users as $user) {
        $userAvatars[$user['id']] = $user['avatar'];
    }
    
После

    $userAvatars = array_column($users, 'avatar', 'id');
    
---

### Не используйте array_merge в циклах

На каждой итерации PHP копирует массив в другой временный массив, что приводит к временному выделению памяти. С каждой последующей итерацией объем используемой памяти увеличивается.

До

    $result = array();
    foreach ($source as $list) {
        $result = array_merge($result, $list);
    }
    
После

    $result = array_merge(...$source);
    
---
