# Конспект для работы с git

## Разные команды

## diff

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

## help

## status
        $ git status #определим состояния файлов
        $ git status -s #сокращенный вывод статуса
## commit

## rm

## remote

## branch

## push

## fetch

## reset & restore

## Наиболее часто употребляемые мной команды