# Помощник для работы с Git

1. Инициализация репозитория с помощью команды git init``(не забудьте сначала перейти в директорию репозитория с помощью `cd`).
(Если вы сделали ошибочный репозиторий, то можно его "разгитить" `rm -rf .git`).
2. Проверить статус `git status`.
3. Добавить файлы в репозиторий `git add --all` (все файлы в репозитории) или `git add .` (вся тенкущая папка) или `git add README.md` (конкретный файл).
4. Делаем коммит `git commit -m 'Мой первый коммит!'`.
5. Просматриваем историю коммитов `git log`.
6. Заходим на GitHub, создаем новый репозиторий, копируем HTTPS или SSH код репозитория. 
7. Привязываем удаленный репозиторий к удаленному, последним параметром вставляем код репозитория `git remote add origin git@github.com:%ИМЯ_АККАУНТА%/first-project.git`.
8. Убедиться, что репозитории связаны `git remote -v`.
9. Отправить изменения на удалённый репозиторий `git push`. В первый раз эту команду нужно вызвать с флагом -u 
и параметрами origin (имя удалённого репозитория) и main или master (название текущей ветки).
Флаг -u свяжет локальную ветку с одноимённой удалённой. Вот так: `git push -u origin master`.
---
При последуюших изменениях репозитория каждый раз повторять 3 (~add~), 4 (~commit~) и 9 (~push~) пункты.