﻿
Определение GoF
Отделите построение сложного объекта от его представления, чтобы тот же
процессы строительства могут создавать разные представления.

Concept
Шаблон Builder полезен для создания сложных объектов с несколькими частями.
Процесс создания объекта должен быть независимым от этих частей; другими словами,
процесс строительства не волнует, как эти части собраны. Кроме того, вы
должен иметь возможность использовать один и тот же процесс построения для создания различных представлений
объектов.
Следующая структура шаблона принимается из книги GoF; см. рисунок

Здесь Product является объектом комплексного объекта. ConcreteBuilder
создает и собирает части объекта продукта путем реализации абстрактного
интерфейс Builder. Объекты ConcreteBuilder строят внутренние представления
продуктов и определяет процесс создания и сборки. Директор
ответственный за создание конечного объекта с использованием интерфейса Builder.

Пример реальной жизни.
Чтобы выполнить заказ для компьютера, различные аппаратные части собраны на основе
предпочтения клиента. Например, клиент может выбрать жесткий диск емкостью 500 ГБ с поддержкой Intel
процессор, а другой клиент может выбрать жесткий диск емкостью 250 ГБ с процессором AMD.

Пример компьютерного мира
Вы можете использовать этот шаблон, если хотите преобразовать один текстовый формат в другой текст
формат, такой как преобразование из RTF в ASCII.

