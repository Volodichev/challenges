## 1. Найдите и исправьте как можно больше ошибок

```
# -*- coding: utf-8 -*-
# from xyz import *

file = r"C:\Users\alex\Desktop\boys.txt"
boys = {'sam':'peters','peter':'johns','michael':'kitton','bob':'marley','fransua':'julien'}


def SomeFUNC(boys={}):

    count = 1
    for x in range(len(boys)):
        boys_names = list(boys.keys())
        if boys_names[x].islower():
            var = boys_names[x]
            boys_names[count] = var[0].upper() + var[1:]
            if var is "peter":
                del boys_names[x]
                print('We delete: ' + var)
            else:
                print("Boy number" + str(x) + " is " + var)
            count = count + 1

    f = open(file, 'w')
    f.write(str(boys))

    print("Coef: " + str(n := int(len(boys))) * 0, sum([(-1) ** i * 1 / (2 ** i) for i in range(n)]), sep='')


SomeFUNC(boys)
```



## 2. Написать тесты для существующего API
_Ресурс:_ API Binance.com

_Инструменты:_ pytest/unittests или анлоги на ваш выбор

_Задача:_ Написать тест для 2-3 основных методов предоставляемых сервисом(например: получение текущих курсов криптовалют)

В тесте обязательно должны присутствовать проверки: кодов состояний, заголовки, полезной нагрузку ответа(том числе на ошибочные запросы) и время ответа(если время больше N -> тест не пройден).

Справка по работе с binance: https://binance-docs.github.io/apidocs/spot/en/#general-info



## 3. Покрыть тестами SELENIUM или браузер.
_Ресурс:_ goldenseed.ru

_Инструменты:_ SELENIUM или анлоги на ваш выбор

Задача:
Написать тест для сайта goldenseed.ru Необходимо реализовать сценарий входа на сайт, найти и перейти на форму обратной связи соискателя работы, заполнение и отправку данных соискателя.



------
Будет плюсом:
Использование docker для поднятия и развертывания dev-среды.



