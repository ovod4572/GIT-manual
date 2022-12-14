# Инструкция для работы с Git и удаленными репозиториями

## 1. Что такое Git?

Git - это одна из реализаций распределенных систем контроля версий, так и удаленные репозитории. Является самой популярной реализацией систем контроля версий в мире.

## 2. Синтаксис разметки языка Markdown

* Жирный текст - ****жирный****. Аналогично ( __ )
* Курсив - **курсив**, ******жирный курсив*** ***. Аналогично ( _ )
* Зачеркнутый текст - ~~ ~~текст~~ ~~
* Выделение заголовка - # в начале строки (шесть градаций. # - самый большой размер букв, ###### - самый маленький).
* Уровень заголовка - = или -
* Нумерованные списки - цифрами с точкой: 1, 2, 3, ...
* Ненумерованные списки - * в начале строки,    либо (- или +)
* Многоуровневые списки - отступ или табуляция (TAB)
* Ссылки и картинки - [текст](ссылка на картинку). Например:
![пустыня зимой](foto.jpg)

## 3. Команды

* clear - очистить терминал
* git_*команда*_--help -

* git_add_*имя файла* - сохранение текущего состояние проекта

* git_branch - список имеющихся веток в репозитории

* git_branch_*имя ветки* -  создание новой ветки

* git_branch_-a -  список удалённых веток

* git_branch_-d_*имя ветки* - удаление ветки

* git_checkout_*имя ветки* - переключение между ветками
* git_checkout_*имя файла* - восстановить файлы рабочего дерева, не подготовленные к коммиту
* git_checkout_-b_*имя ветки* - создание ветки и переход на неё
* git_commit_-m_"*Пояснение*" - фиксация изменений в репозиторий
* git_commit_--amend_-m *Изменения* - внести изменения в последний коммит
* git_clone_*URL-адрес репозитория* - клонировать репозиторий во вновь созданный католог
* git_diff - вывод изменений между сохраненным и последним файлом
* git_fetch_*URL-адрес репозитория* - загружает коммиты, файлы и ссылки из удаленного репозитория в ваш локальный репозиторий
* git_init - создание в директории пустой репозитории
* git_log  - вывод списка изменеий
* git log_-p - вывод изменений, внесённых в каждый файл
* git_log_--graph - выводит изменения репозитории в виде дерева с псевдографикой
* git_merge_ *имя ветки* - слияние изменений
* git_merge_--abort - прервать слияние
* git_mv_*имя файла1*_*имя файла2* - переименование файла
* git_pull - получение изменений и слияние с локальной версией
* git_pull_request - предложение изменения кода в чужом репозитории  
* git_push - отправка локальной версии в удаленный репозиторий
* git_revert_ *индекс* - откатить последний коммит
* git_reset_*путь к файлу* - восстановить подготовленный файл рабочего дерева
* git_rm_dirnam/*имя файла* - удаление файла и индекса из текущего рабочего дерева
* git_show_*идентификатор* -  полный список изменений, внесённых конкретным коммитом
* git_status - отображает список изменённых, добавленных и удаленных файлов

## 4. Подготовка репозитория

Для создания репозитория необходимо выполнить команду git init в папке с репозиторием и у Вас создаться репозиторий (появится скрытая папка .git)

* Для удобства работы в репозитории создать файлы:
  * .gitignore
  * readme.md

## Использование GitHub

* Настройка :
    1. Создать аккаунт на GitHub.com.
    2. Создать локальный репозиторий.
    3. Настроить локальный и удаленный репозиторий. При создании нового репозитория GitHub даст подсказки.
    4. Отправить (push) локальный репозиторий в удаленный (на GitHub), при этом, нужно будет авторизоваться на удаленном репозитории.
    5. Провести изменения "с другого компьютера".
    6. Скачать (pull) актуальное состояние из удаленного репозитория.

* Копирование репозитория:
    1. Делаем форк (fork) интересующего репозитория.
    2. Делаем git clone для нашей версии этого репозитория.
    3. Создаем ветку с предлогаемыми изменениями.
    4. Производим все изменения в этой ветке.
    5. Отправляем эти изменения на свой аккаунт (push).
    6. В окне на GitHub появляется возможность отправить pull request.
