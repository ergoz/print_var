Print Var
=========

Функция для удобочитаемого вывода значений переменных на экран в php.

Плюшки:
* Переменная распечатывается в диалоговом окне, не ломая вёрстку сайта,
* В шапке диалогового окна выводится информация о файле и строке в файле, в которой вызвана функция,
* Вместе со значением переменной выводится информация о её типе,
* Значение массивов, объектов и функций можно сворачивать
* Для переменных типа объект выводится информация о публичных полях и функциях,
* Для функций выводится список параметров вместе со значениями по-умолчанию.

<p align="center">
  <img src="https://github.com/xescoder/print_var/blob/master/example.png?raw=true">
</p>

Использование
-------------

Для использования достаточно:

1.  Подключить print_var.php где-нибудь в начале страницы,
2.  Вызвать print_var, передав ей переменную.

`````php
// Подключить print_var
include 'print_var.php';

// Вызвать функцию
$str = 'variable';
print_var($str);
`````

Деактивация
-----------

В случае если вы забыли удалить вызов print_var его можно быстро деактивировать, определив константу DISABLE_PRINT_VAR

`````php
// Деактивация print_var
define('DISABLE_PRINT_VAR', true);
`````