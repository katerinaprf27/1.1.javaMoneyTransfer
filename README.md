# Отчёт о тестировании приложения "Money Transfer" #

## Краткое описание ##

27.01.2021 было проведено функциональное, позитивное тестирование установки приложения Money Transfer.

На тестирование затрачено: 1 час.

В результате тестирования выявлены следующие *дефекты*:

При пополнении счета в приложении, использовав переменную "int", получилось отрицательное число -1794967296, чего быть не должно, так как суммировались два положительных числа.

Тестирование производилось в следующем окружении:
* MacOS x64
* Java version "11.0.9.1"
* IntelliJ IDEA

## Описание тестов ##

Было проведено функциональное, позитивное тестирование установки приложения Money Transfer. 
С целью проверки как работает оператор *"сложение"* и переменная *"int"* c  цифрами 2_000_000_000 и 500_000_000.

## Результаты ##

1. Данное тестирование оказалось 100% неуспешным тестом.

2. [Неверный расчет баланса при пополнении счета клиента](https://github.com/katerinaprf27/1.1.javaMoneyTransfer/issues/3)

# Общие рекомендации #

По итогам тестирования рекомендую при разработке приложений, где планируются использоваться большие цифры брать переменную с запасом - *"long"*.