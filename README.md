# Autotexts
Решение для Directum RX 4.6

Возможности решения

Отдельный справочник Автотексты с разграничением прав доступа, содержащий автотексты для использования в задачах и заданиях (разграничение реализовано с использованием записей справочника Области использования).

Состав решения

Модуль Автотексты.

Справочник Автотекст (Autotext).

Справочник Область использования (AutotextUsageArea)	

Новая роль «Создание автотекстов». При инициализации выдаются права на создание записей и заполнение свойств справочника Автотекст и на чтение записей справочника Область использования.

Новая роль «Использование автотекстов». При инициализации выдаются права на чтение записей справочника Автотекст и на чтение записей справочника Область использования.

Локализация новых элементов разработки.

Варианты расширения функциональности на проектах

Добавление множественного выбора областей использования для автотекстов;

Добавление фильтрации использования автотекстов по подразделениям.

Архитектурно неочевидные моменты


Внедрение решения

При внедрении решения необходимо произвести следующие действия: 

Определить набор областей использования и создать в инициализации соответствующие записи справочника Область использования;

В перекрытиях задач/заданий добавить кнопку для добавления автотекста, которая будет вызывать серверную функцию GetAutotexts модуля автотексты, с указанием Guid области использования соответствующей задаче/заданию из которой вызывается функция.