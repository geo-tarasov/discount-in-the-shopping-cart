# Скидка в корзине. Расширение для сайта на Tilda
## Задача
В конструкторе сайтов Tilda нет встроенного функционала для настройки скидки по количеству товара. Нужно было:

1. Применять скидку, когда количество товаров в корзине будет 3 шт. или больше
2. Когда в корзине ровно 2 шт. товаров, предложить добавить третий товар для получения скидки
3. Дополнительно применять скидку по промокоду

## Решение
За основу было взято готовое решение для добавления скидки в зависимости от кол-ва товаров в корзине (https://mo-ti.ru/mydiscount), но его предстояло доработать.

Во-первых, одновременно с этим готовым решением нельзя использовать встроенное в конструктор тильды поле промокодов, потому что тильда не позволяет пробивать две скидки одновременно

Во-вторых, нужно было выводить уведомление при добавлении двух товаров, что тоже не реализовано в готовом решении

Для суммирования скидок за 3 товара (20%) и за введенный промокод (20%) я решил создать свое, не из конструктора тильды поле промокода, и проверял промокод сразу на клиентской части. Если промокод введен верно и в корзине три товара - пробивалась скидка 40%, если одно из условий не выполнено, пробивалась скидка 20%. Эту реализацию мы сразу обговорили с заказчиком, она его полностью устроила.

## Результат
<img src="https://github.com/geo-tarasov/discount-in-the-shopping-cart/assets/88404017/dc45025b-5545-4223-989d-c84651b06321" width="200">&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;<img src="https://github.com/geo-tarasov/discount-in-the-shopping-cart/assets/88404017/43c97f66-58e7-4be7-807e-5b65f7d3a15e" width="200" style="margin-left:20px">

## Отзыв о работе
https://github.com/geo-tarasov/discount-in-the-shopping-cart/assets/88404017/6ade4013-7300-4c6e-a206-46e06e2a2ac6

###### Код представлен в ознакомительных целях, не для свободного использования
