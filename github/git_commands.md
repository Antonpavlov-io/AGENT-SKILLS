# Справочник: Команды Git

## Базовые операции
- `git clone <URL>` — клонировать репозиторий
- `git status` — статус рабочего дерева
- `git diff` — изменения относительно последнего коммита
- `git add <file>` — добавить файл в индекс
- `git commit -m "message"` — создать коммит
- `git push origin <branch>` — отправить ветку в remote
- `git pull origin <branch>` — получить и слить изменения из remote
- `git fetch` — получить изменения без слияния

## Ветки
- `git branch <name>` — создать ветку
- `git switch <branch>` — переключиться на ветку
- `git checkout -b <name>` — создать ветку и переключиться
- `git merge <branch>` — слить ветку в текущую
- `git rebase <branch>` — перенести коммиты поверх другой ветки
- `git branch -d <name>` — удалить ветку локально

## История коммитов
- `git log --oneline --graph` — компактный граф коммитов
- `git log --author="name"` — коммиты конкретного автора
- `git log --since="YYYY-MM-DD"` — коммиты после указанной даты
- `git log --grep="text"` — поиск по сообщению коммита
- `git log --stat` — статистика изменённых файлов по коммитам

## Отмена изменений
- `git stash` — временно отложить незакоммиченные изменения
- `git stash pop` — восстановить отложенные изменения
- `git revert <commit>` — отменить коммит новым коммитом (безопасно)
- `git reset --hard <commit>` — откатить до коммита (деструктивно; с осторожностью)
- `git cherry-pick <commit>` — применить конкретный коммит в текущую ветку

## Работа с remote
- `git remote` — список remote-репозиториев
- `git remote add <name> <URL>` — добавить remote
- `git remote remove <name>` — удалить remote
- `git tag <name>` — создать тег на текущем коммите
- `git push origin <tag>` — отправить тег в remote
