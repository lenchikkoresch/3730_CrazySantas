# Инструкция для работы с Git и удалёнными репозиториями

## Что такое Git?
Git - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.

## Для чего нужен Git?
Чаще всего его используют для кода, но можно и для других файлов. Например, для картинок - полезно для дизайнеров. С помощью Git-a можно откатить проект до более старой версии, сравнивать, анализировать или сливать изменения в репозиторий.

Настройка Git-а
--
> Установим имя пользователя (Вместо <ваше_имя> можно ввести, например, Grisha_Popov, ковычки оставляем)
>> git config --global user.name "<ваше_имя>"

> Установим установим email (Принцип такой же)
>>git config --global user.email "<адрес_почты@email.com>" 

> Проверить настройки командой 
>> cat .gitconfig

## Подготовка репозитория
Для создание репозитория необходимо выполнить команду *git init*  в папке с репозиторием и у Вас создаться репозиторий (появится скрытая папка .git)

### Что такое репозиторий
Репозиторием называют хранилище вашего кода и историю его изменений. Git работает локально и все репозитории хранятся в определенных папках на жестком диске.

### Хранение репозиторий в интернете
Так же репозитории можно хранить и в интернете. Обычно для этого используют три сервиса:

* GitHub
* Bitbucket
* GitLab 

## Создание коммитов

### Git add
Для добавления измений в коммит используется команда *git add*. Чтобы использовать команду *git add* напишите *git add <имя файла>*

### Просмотр состояния репозитория
Для того, чтобы посмотреть состояние репозитория используется команда *git status*. Для этого необходимо в папке с репозиторием написать *git status*, и Вы увидите были ли измения в файлах, или их не было.

### Создание коммитов
Для того, чтобы создать коммит(сохранение) необходимо выполнить команду *git commit*. Выполняется она так: *git commit -m "<сообщение к коммиту>*. Все файлы для коммита должны быть ***ДОБАВЛЕНЫ*** и сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***.

## Перемещение между сохранениями
Для того, чтобы перемещаться между коммитами, используется команда *git checkout*. Используется она в папке с пепозиторием следующим образом: *git checkout <номер коммита>*

## Журнал изменений
Для того, чтобы посмтреть все сделанные изменения в репозитории, используется команда *git log*. Для этого достаточно выполнить команду *git log* в папке с репозиторием

## Ветки в Git

### Создание ветки

Для того, чтобы создать ветку, используется команда *git branch*. Делается это следующим образом в папке с репозиторием: *git branch <название новой ветки>*

## Слияние веток

Для того чтобы дабавить ветку в текущую ветку используется команда *git merge <name branch>*

## Удаление веток
Для удаления ветки ввести команду "git branch -d 'name branch'"
