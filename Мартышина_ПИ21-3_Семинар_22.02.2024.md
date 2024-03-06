## АПИ автотесты на Python
### Первый запуск
![image](https://github.com/lisatheelsa/upravleniye_kachestvom_programmnih_system/assets/101552146/8af296b9-186f-4384-860d-1cea4dde6bda)

### Обнаружение ошибок
##### Ошибка "TypeError: unsupported operand type(s) for |: 'type' and 'NoneType'" в классе ObjectUpdateOutSchema и ObjectCreateOutSchema возникает из-за использования оператора | в аннотации типа. 
##### В данном случае, оператор | пытается объединить тип str и NoneType, что не поддерживается в Python 7.
![image](https://github.com/lisatheelsa/upravleniye_kachestvom_programmnih_system/assets/101552146/52e3304c-3d7f-4534-b7a1-3870b6db16d2)

### Исправление ошибок
##### Уберём оператор | None из аннотаций типов для name и data, так как класс BaseModel из модуля pydantic уже поддерживает необязательные поля. 
##### Затем, изменим аннотацию типа для createdAt и updateAt на str.
![image](https://github.com/lisatheelsa/upravleniye_kachestvom_programmnih_system/assets/101552146/17716b9d-651a-41db-9279-275817985208)
![image](https://github.com/lisatheelsa/upravleniye_kachestvom_programmnih_system/assets/101552146/b16a9bc2-64ea-414b-b6dc-eda223405e6d)

### Работа 5 АПИ методов прошла проверку 16-ю тестами.
![image](https://github.com/lisatheelsa/upravleniye_kachestvom_programmnih_system/assets/101552146/600c77af-609d-46c7-a1ab-3acfef6b8ee4)

