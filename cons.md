# Инструкция по работе с гит для начинающих

Цитата из [Википедии](https://ru.wikipedia.org/wiki/Git "Ссылка на Гит в Википедии") о Гит:
>Git (произносится «гит») — распределённая система управления версиями. Проект был создан Линусом Торвальдсом для управления разработкой ядра Linux, первая версия выпущена 7 апреля 2005 года. На сегодняшний день его поддерживает Джунио Хамано.

## Основные команды Git:
 - **git --version** - вывод информации о версии Гита.
 - **git init** - инициализация каталога для отслеживания Гитом (делает из каталога репозиторий).
 - **git status** - проверка статуса отслеживания.
 - **git add "file"** - добавление файла для отслеживания.
 - **git commit -m "comment"** - сохраняет слепок репозитория с добавлением комментария.
 - **git log** - выводит журнал изменений.
 - **git checkout "id"** - возврат к определенной версии.
 - **git checkout master** - переключение в текущее состояние (возврат к актуальной версии).
 - **git diff** - выводит записанные изменения в файле (до коммита).
 - **git config --global user.name "name"** - задаёт имя пользователя Гита.
 - **git config --global user.email "E-mail"** - задаёт E-mail пользователя Гита.
 - **git config --global --list** - выводит имя и E-mail пользователя Гита.
 - **git switch -** - аналог **git checkout master**.
 

 ## Команды для использования механизма ветвления:
 - **git branch** - просмотр текущей ветки (выделяется звёздочкой) и других созданных.
 - **git branch "name"** - создание новой ветки.
 - **git checkout "name"** - переход на другую ветку.
 - **git merge "name"** - слияние ветки *name* с текущей.
 - **git branch -d "name"** - удаление ветки.
 - **git log --graph** - визуализация журнала изменений. Добавляется отображение дерева веток.

*Под веткой принято понимать независимую последовательность коммитов в хронологическом порядке.*

 ## Описание методов слияния:
**fast-forward** - прямое слияние, когда ветка *master* сразу перемещается на коммит из соседней ветки.
 
