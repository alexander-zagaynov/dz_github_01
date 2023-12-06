# Test-Rep-1

Hello word!
Начинаем углубленное изучение GIT HUB

Hello word!
Начинаем углубленное изучение GIT HUB

1 **скачали репозиторий** с  git hub / Test-Rep-1
*git clone https://github.com/alexander-zagaynov/Test-Rep-1.git
отключаемся от репозитория git remote remove origin
проверяем git remote -v*

2 **отправляем в другой репозиторий** в git hub / Test-Rep-2
*подключаемся к удаленному репозиторию
git remote add origin https://github.com/alexander-zagaynov/Test-Rep-2.git

отправляем в удаленный репозиторий
git push -u origin main*

3 **Связываем 2 удаленных репозитория**
*git remote add source https://github.com/alexander-zagaynov/Test-Rep-1.git
проверяем: git remote -v*
**Должна появиться такая информация по двум репозиториям**
alexanderzagaynov@MacBook-Pro-alexander Test-Rep-1 % git remote -v
origin  https://github.com/alexander-zagaynov/Test-Rep-2.git (fetch)
origin  https://github.com/alexander-zagaynov/Test-Rep-2.git (push)
source  https://github.com/alexander-zagaynov/Test-Rep-1.git (fetch)
source  https://github.com/alexander-zagaynov/Test-Rep-1.git (push)

Ошибка_неполучилось сделать commit
*alexanderzagaynov@MacBook-Pro-alexander Test-Rep-1 % git commit -m "Change line"
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean*


Conflict
alexanderzagaynov@MacBook-Pro-alexander Test-Rep-1 % git push -u origin first
Enumerating objects: 15, done.
Counting objects: 100% (15/15), done.
Delta compression using up to 4 threads
Compressing objects: 100% (9/9), done.
Writing objects: 100% (9/9), 1.40 KiB | 1.40 MiB/s, done.
Total 9 (delta 3), reused 0 (delta 0)
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
To https://github.com/alexander-zagaynov/Test-Rep-2.git
   211e400..bee7c77  first -> first
Branch 'first' set up to track remote branch 'first' from 'origin'.

 Исправление конфликта
 сделаны: изменения в удаленом GITHUB
 и изменения в локальном ПК
**git pull origin first**
From https://github.com/alexander-zagaynov/Test-Rep-2
  branch            first      -> FETCH_HEAD
Already up to date.*

Создание конфликта
