1 задача
// Объявляем переменные
let product = 'Печенье «Юбилейное», 1 кг';
let inBasket = true;
let quantity = 5;
 
// Проверяем, находится ли товар в корзине
if (inBasket) {
    console.log(`{quantity} x {product}`);
}

2 задача
// Создаём переменные и заполняем тестовыми данными
let accountStatus = 'premium'; // может быть: 'extended', 'premium', 'vip'
let username = 'Иван';
let cashbackPercentage;

// 2. Определяем размер кэшбека по статусу
switch (accountStatus) {
    case 'extended':
        cashbackPercentage = 15;
        break;
    case 'premium':
        cashbackPercentage = 20;
        break;
    case 'vip':
        cashbackPercentage = 30;
        break;
    case 'regular':
        cashbackPercentage = 10; // обычный аккаунт
}

// 3. Формируем и выводим результат
let statusLabel = ['regular', 'extended', 'premium', 'vip'] .includes(accountStatus) ? accountStatus : 'regular';

console.log('{username} | {statusLabel} аккаунт`);
console.log(`Вы получаете ${cashbackPercentage} % с покупок на бонусный счёт`);

 Пример вывода для `accountStatus = 'premium'`:

Иван | premium аккаунт
Вы получаете 20 % с покупок на бонусный счёт
```

3 задача
if ((user = 'admin'))
заменилА присваивание
=
на строгое сравнение
===
.
- В строке приветствия админа исправила
/n
на правильный перевод строки
\\n
.
- В строке вывода количества заказов исправила опечатку
errorOreders
на
errorOrders
.
- Изменила условие для вывода информации о заказах: теперь сообщение появляется, если есть новые заказы (
newOrders > 0
), а не только если их больше, чем ошибочных.
- В предупреждающем сообщении исправила логику: теперь оно срабатывает, если количество ошибочных заказов равно общему количеству новых заказов.

