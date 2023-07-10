# GR_4406


# Инструкция по работе с Git на облегченном языке разметки Markdown

## Что такое Git?
Git - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире. [Скачать можно по ссылочке здесь.](https://git-scm.com/)

>Git (произносится «гит»[7]) — распределённая система управления версиями. Проект был создан Линусом Торвальдсом для управления разработкой ядра Linux, первая версия выпущена 7 апреля 2005 года. -Википедия

![Лого Гита](https://git-scm.com/images/logo@2x.png)

## Подготовка репозитория
Для создание репозитория необходимо выполнить команду *git init* в папке с репозиторием и у Вас создаcтся репозиторий (появится скрытая папка .git).

## Git add
Для добавления измений в коммит используется команда *git add*. Чтобы использовать команду *git add* напишите *git add <имя файла>*

## Просмотр состояния репозитория
Для того, чтобы посмотреть состояние репозитория используется команда *git status*. Для этого необходимо в папке с репозиторием написать *git status*, и Вы увидите были ли измения в файлах, или их не было.

## Создание коммитов
Для того, чтобы создать коммит(сохранение) необходимо выполнить команду *git commit*. Выполняется она так: *git commit -m "<сообщение к коммиту>*. Все файлы для коммита должны быть ***ДОБАВЛЕНЫ*** и сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***.

## Перемещение между сохранениями
Для того, чтобы перемещаться между коммитами, используется команда *git checkout*. Используется она в папке с репозиторием следующим образом: *git checkout <номер коммита>*.

git checkout master - переносит нас на ветку master

## Журнал изменений
Для того, чтобы посмотреть все сделанные изменения в репозитории, используется команда *git log*. Для этого достаточно выполнить команду *git log* в папке с репозиторием. Для каждого коммита есть свой идентификационный номер. Чтобы переходить от коммита к коммиту достаточно ввести 4 первые символа к команде checkout.

**Еще некоторые команды:**

* git help
* git diff
* git clone

1. Подсказка по командам
2. Наглядно показывает разницу коммитов и веток
3. Клонирует репозиторий


## Полезные команды
`git checkout -b branch_name` -для создания ветки с переходом на нее

`git commit -am "commit_message"` -коммит и индексация выполняются за одну команду

`git log —graph —oneline` -отображает лог графически и коротко




## Ветки в Git
Ветка - это набор commit, которые идут друг за другом. У ветки есть название, основную ветку чаще всего называют master . Если говорить простыми словами, то ветка master - это наш проект.
Другие ветки - это отдельное место для реализации нового функционала или исправление багов (ошибок) нашего проекта. То есть, с отдельной веткой вы делаете что угодно, а затем сливаете эти изменения в основную ветку master.

Чтобы посмотреть сколько у нас на данный момент веток и какая из них текущая (в которой мы работаем) набираем команду *git branch*. Новые ветки создаем из ветки master. Для этого достаточно команду просто применить в папке с репозиторием.

### Создание ветки
Для того, чтобы создать ветку, используется команда *git branch*. Делается это следующим образом в папке с репозиторием: *git branch <название новой ветки>*.

**Чтобы перейти от одной ветки к другой - *git checkout < name>*.**

### Слияние веток
Когда нас черновик полностью устраивает, мы можем перенести эту ветку в master. Для того чтобы дабавить ветку в текущую ветку используется команда *git merge <name branch>*. Команду выполняем из той ветки, в которую нужно перенести наш черновик.

### Удаление веток
Если ветка - черновик больше не нужна, то можем ее удалить.
"git branch -d 'name branch'" для удаления ветки
-------------------------------------—

## Полезные команды
`git checkout -b branch_name` -для создания ветки с переходом на нее

`git commit -am "commit_message"` -коммит и индексация выполняются за одну команду

`git log —graph —oneline` -отображает лог графически и коротко


## ****Работа с удаленными репозиториями*

### Настраиваем совместную работу

1. Создать аккаунт на GitHub.com
2. Создать локальный репозиторий
3. “Подружить” ваш локальный и удалённый репозитории. GitHub при создании нового репозитория подскажет, как это можно сделать
4. Отправить (push) ваш локальный репозиторий в удалённый (на GitHub), при этом, возможно,
вам нужно будет авторизоваться на удалённом репозитории
5. Провести изменения “с другого компьютера”
6. Выкачать (pull) актуальное состояние из удалённого репозитория


## Основые команды для данной работы:

`` git clone`` - Эта команда позволяет склонировать внешний репозиторий на ПК

``git pull`` - Эта команда позволяет скачать все из текущего репозитория и автоматически сделать merge с нашей версией

``git push`` - Эта команда позволяет отправить нашу версию репозитория на внешний репозиторий. *требует авторизации* на внешнем репозитории


## __Pull request__

1. Делаем fork репозитория
2. Делаем clone СВОЕЙ версии репозитория
3. Создаем новую ветку и в НЕЕ вносим свои изменения
4. Фиксируем изменения (делаем коммиты)
5. Oтправляем свою версию в свой GitHub
6. На сайте GitHub нажимаем кнопку pull request


## Создание удаленного репозитория
Создадим новый репозиторий на GitHub. Для этого на сайте GitHub кликните на значок плюса справа сверху или перейдите по ссылке.

![Перед нами откроется следующая форма:](Create-repository.png) 


* ``Owner`` (владелец) – выбрать персональный аккаунт, который будет иметь полный доступ к данному репозиторию.
* ``Repository`` name (название репозитория) – при названии репозитория принято использовать PascalCase (составные слова с заглавной буквы) и kebab-case (составные слова через дефис).
* ``Description`` (описание) – описание проекта.
* ``lic`` – кто угодно может просматривать репозиторий, но коммитить смогут только те аккаунты, которым вы предоставите доступ.
* ``Private`` – никто, кроме вас, не сможет коммитить или просматривать данный репозиторий без права доступа.
* ``Add a README file`` – создает readme.md файл, который нужен для добавления длинного описания.

После нажатия Create repository нас перекинет на страницу нашего нового репозитория.

![.](github.jpd.png)
*Пример созданного репозитория на GitHub*

