- Инициализация репозитория
```bash
git init
```

- Проверка состояния репозитория
```bash
git status
```

- Подготовить файлы к сохранению
```bash
git add <file_name>
```

*Можно и ```git add . или git add --all```, но лучше делать с каждый файлом,*   
*т.к. можно запушить что-то лишнее*

```mermaid
graph LR;
  untracked -- "git add" --> staged;
``` 

- Выполнить коммит с сообщение в командной строке
```bash
git commit -m "<message>"
```

- Выполнить коммит с оформлением сообщения в редакторе
```bash
git commit
```

```mermaid
graph LR;
  staged    -- "git commit"     --> tracked/comitted;
``` 

- Просмотреть историю коммитов полностью
```bash
git log
```
- Просмотреть историю коммитов однострочно
```bash
git log --oneline
```

```mermaid
graph LR;
  tracked/comitted -- "git push" --> tracked;
``` 