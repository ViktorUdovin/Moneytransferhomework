## Отчёт о тестировании приложения "Money transfer"

### Краткое описание

Для тестирования нашего приложения я решил протестировать разные математические значения в коде, чтобы прийти к верному решению. Я использовал: Сложение,Вычитание и Деление. При использовании данных функций, стало понятно, что наша ошибка заключается в использовании переменной Int, вместо переменной long.

### Описание тестов

Функциональное тестирование приложения.
Для тестирования я использовал разные матиматические функции:
1. Сложение
2. Вычитание
3. Деление

### Результаты:
Тестирование с использованием вычитания и деления прошло позитивно, тотал принимает верные значения.
Тестирование основной функции - сложения, прошло негативно, так как тотал принимает неверное значение.

#### Баг-репорт:
[Неверная сумма при сложении "счета" и "пополнения счета" в Money transfer #1](https://github.com/ViktorUdovin/Moneytransferhomework/issues/1)

### Общие рекомендации

Я считаю, что дело в том, что при сложении, переменная Int не может вместить в себя число "2500000000", от этого и возникает баг. Нам следует заменить переменную Int на переменную log, и баг будет исправлен.