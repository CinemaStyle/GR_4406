# GR_4406
# **Инструкция для работы с Git и удаленными репозиториями**

## **Что такое Git?**

Git — это система контроля версий, которая помогает отслеживать историю изменений в файлах.

**Что такое репозиторий Git?**

Репозиторий — это все файлы, находящиеся под контролем версий, вместе с историей их изменения и другой служебной информацией

**Создание и настройка**
* git init - инициализирует новый репозиторий
* git clone *url* - клонирует существующий репозиторий
* git config - настраивает глобальные настройки Git
* git remote add *name url* - добавляет удаленный репозиторий

**Основные операции**
* git add *file* - добавляет файлы в индекс
* git commit -m *"message"* - создает коммит с сообщением
* git commit -am *"message"* - создает коммит с сообщением без команды add
* git log --graph - вывод дерева коммитов
* git log oneline --graph - вывод дерева коммитов в одну строку
* git status - выводит состояние рабочей директории
* git diff - выводит различия между файлами

**Ветвление и слияние**
* git branch - выводит список веток
* git branch *name* - создает новую ветку
* git branch -b *name* - переход на новую ветку 
* git branch -d *name* - удаляет ветку
* git branch -a *name* - показыввает удаленные ветки
* git checkout *branch* - переключается на указанную ветку
* git merge *branch* - сливает указанную ветку с текущей

**Удаление и отмена изменений**
* git reset HEAD *file* - отменить индексацию файла
* git merge --abort - отменить процесс слияния
* git rm *file* - удаляет файл из индекса и рабочей директории
* git reset *file* - отменяет изменения в файле
* git revert *commit* - создает новый коммит, отменяющий изменения
* git clean	- удаляет непроиндексированные файлы и директории


*Справочно*

_**Руководство по синтаксису Markdown**_

1. Абзацы создаются при помощи пустой строки. Если вокруг текста сверху и снизу есть пустые строки, то текст превращается в абзац.

2. Чтобы сделать перенос строки вместо абзаца, нужно поставить два пробела в конце предыдущей строки.

3. Заголовки отмечаются диезом `#` в начале строки, от одного до шести.

4. Вложенные пункты создаются четырьмя пробелами перед маркером пункта.

5. Цитаты оформляются как в емейлах, с помощью символа `>`.

6. Чтобы создать таблицу можно использовать обычные способы форматирования внутри ячеек. Столбцы могут быть выровнены также по правому краю или по центру с помощью двоеточий в строке отделяющей заголовок таблицы от остального текста.

7. Есть два способа создать ссылку на какой-либо web-ресурс: первый - поместить ссылку прямо в текст. Заключите текст, который пользователь должен видеть и который будет выглядеть как ссылка в квадратные скобки, а URL страницы в круглые так, чтобы комплекты скобок были написаны слитно. Также вы можете добавить дополнительное описание, заключив его в кавычки и поместив после URL.
8. Картинки помещаются на страницу точно таким же образом, как и web-ссылки, но предваряются восклицательным знаком.