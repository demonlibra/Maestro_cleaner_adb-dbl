# Сценарий очистки Maestro\Projects от файлов ADB и DBL
  
## Использование
1. Скачайте архив, используя ссылку [Clone or download - Download ZIP](https://github.com/demonlibra/phpBB-ext-sitemaker-3.2-translate-rus/archive/master.zip).  
2. Извлеките файл `Maestro_Cleaner_adb&dbl.vbs` и разместите его
   * на рабочем столе - для ручного запуска
   * в автозапуске - для автоматического запуска при каждом включении станка.

## Параметры
В начале файла указаны основные параметры.  
Открыть файл `Maestro_Cleaner_adb&dbl.vbs` можно в любом тесктовом редакторе, например в блокноте.  
Переменная `path_Maestro_Project` должна содержать путь к каталогу с проектами Maestro.

Обычно этот путь:  
`path_Maestro_Project = "C:\Program Files (x86)\Scm Group\Maestro\Projects"`

На старых станках с 32-х разрядной операционной системой:  
`path_Maestro_Project = "C:\Program Files\Scm Group\Maestro\Projects"`

## Шаблон для поиска файлов
Поиск файлов для удаления осуществляется по шаблону регулярного выражения:  
`mask = "(_adb.|_dbl.)"`

Добавьте символы для поиска и разделите их вертикальной чертой, если необходимо удалять еще какие-то файлы:  
`mask = "(_adb.|_dbl.|log|test)"`

## Поддержка
Вопросы Вы можете задать на форуме [forum.tecnocom-ug.ru](http://forum.tecnocom-ug.ru/viewtopic.php?f=153&t=4208).

# Script to clean Maestro\Projects from ADB and DBL files

## Use
1. Dowload archive [Clone or download - Download ZIP](https://github.com/demonlibra/phpBB-ext-sitemaker-3.2-translate-rus/archive/master.zip).  
2. Extract the file `Maestro_Cleaner_adb&dbl.vbs` and put it on the 
   * Desktop (for manual launch)
   * or Startup menu (for automatic launch every time the machine is turned on).

## Parameters
You can open the file `Maestro_Cleaner_adb&dbl.vbs` in any text editor, for example in Notepad.  
The variable `path_Maestro_Project` should contain the path to the directory with Maestro projects.

Usually this path:  
`path_Maestro_Project = "C:\Program Files (x86)\Scm Group\Maestro\Projects"`

On old machines with a 32-bit operating system:  
`path_Maestro_Project = "C:\Program Files\Scm Group\Maestro\Projects"`

## Mask for searching
Regular expression used for searching files which will be delete:  
`mask = "(_adb.|_dbl.)"`

If you need to delete other files, add symbols to searching. "|" is a default item separator:  
`mask = "(_adb.|_dbl.|log|test)"`

## Support
You can post your questions on the forum [forum.tecnocom-ug.ru](http://forum.tecnocom-ug.ru/viewtopic.php?f=153&t=4208).
