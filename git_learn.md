# Конспект для работы с git

## Разные команды
        $ git --version #версия
        $ git clone https://github.com/libgit2/libgit2 #клонируем каталог с сайта
        $ git add README #отслеживание новых файлов можно через пробел много файлов либо $ git add . Тогда все или *
        $ git mv [оригинальный файл] [новое имя] #переименовать файл
        $ git init #инициализируем гид
        $ git show [коммит] #Выводит информацию и показывает изменения в выбранном коммите
        #добавление файла в индекс означает для Git , что все конфликты в нем исправлены.
        q - выйти

## diff
    $ git diff #что мы изменили но не проиндексировали
    $ git diff --staged #что мы индексировали что войдет в следующий коммит (--staged и--cached синонимы)
## log
        $ git log #отобразит историю только для текущей ветки
        $ git log --all #чтобы посмотреть историю по всем веткам
        $ git log -p -2 #-p или --patch показывает разницу внесенную в каждый коммит -2 выводит только 2 записи. 
        $ git log --oneline --decorate --graph --all #покажет историю ветвления
## checkout
        $ git checkout testing #переключится на ветку
        $ git checkout -b <newbranchname> #создать новую ветку и сразу на нее переключиться
            
        $ git checkout -b iss53
            
        $ git checkout -- CONTRIBUTING.md #отменить изменения в файле, вернутся к предыдущему коммиту, удалит все изменения, Внимательность!!!
## config
    $ git config --list #проверка всех настроек
    $ git config user.name #посмотреть в настройках имя (пример)
    $ git config --global user.name "John Doe" #имя
    $ git config --global user.email johndoe@example.com #эл.почта
    $ git config --global init.defaultBranch main #изменение название главной ветки по умолчанию
    $ git config --global core.editor emacs #выбор редактора 

## help
    $ git help <команда> #получить помощь, открывается браузер
    $ git <команда> --help #получить помощь, открывается браузер
    $ git add -h #краткая инструкция по использованию

## status
        $ git status #определим состояния файлов
        $ git status -s #сокращенный вывод статуса
## commit
        $ git commit #эта команда откроет выбранный нами текстовый редактор
        $ git commit -m "Story 182: fix benchmarks for speed" #создать коммит с текстовым сообощением, использую двойные кавычки (рекомендуется)
        $ git commit -a -m 'Add new benchmarks' #создать коммит игнорирую создание индекса, сразу на прямую.
        $ git commit --amend #внести изменения в последний коммит
## rm
        $ git rm [файл] #Удаляет конкретный файл из рабочей директории и индексирует его удаление
        $ git rm --cached [файл] #Убирает конкретный файл из контроля версий, но физически оставляет его на своём месте
        $ git rm log/\*.log #можно удалять каталоги и шаблоны или так $ git rm \*~
## remote

## branch

## push

## fetch

## reset & restore

## Наиболее часто употребляемые мной команды
        git init
        git add [файл]
        git commit -m "комментарий"
        git branch
        git branch [имя файл] #создать ветку
        git branch -d [имя файла] #удалить ветку
        git status
        git log --oneline --graph
        git checkout [название ветки]
        git merge