Подготовь и опубликуй изменения в GitHub. Репозиторий: `https://github.com/flashkate/tutor-report-generator`

**Шаг 1 — Проверь что изменилось**
```bash
git diff --stat
git status
```

**Шаг 2 — Убедись, что приватные данные не попадут в коммит**
```bash
git status
```
Файлы из `raw-data/` не должны быть в списке. Если есть — не добавляй их.

Также проверь, что API key не захардкожен:
```bash
grep -n "sk-ant-" index.html
```

**Шаг 3 — Добавь файлы в коммит**
```bash
git add index.html README.md .gitignore CLAUDE.md
```
Только явные файлы, не `git add .`

**Шаг 4 — Создай коммит**
Сформулируй краткое сообщение на русском или английском (до 72 символов) — что именно изменилось и зачем. Примеры:
- `fix: исправить рендеринг красного светофора`
- `feat: добавить поддержку .docx файлов`
- `docs: обновить README — добавить roadmap`

```bash
git commit -m "твоё сообщение"
```

**Шаг 5 — Запуши**
```bash
git push
```

После пуша выведи ссылку на репозиторий: `https://github.com/flashkate/tutor-report-generator`
