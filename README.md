# Family Tree — GitHub Pages

Минимальный статический вариант без БД и backend.

## Файлы

- `index.html` — сайт.
- `family.json` — все данные семейного древа.
- `.nojekyll` — говорит GitHub Pages не обрабатывать сайт через Jekyll.

## Как запустить

1. Создай новый public-репозиторий на GitHub.
2. Загрузи в корень эти три файла.
3. Открой `Settings → Pages`.
4. В `Build and deployment` выбери `Deploy from a branch`.
5. Branch: `main`, folder: `/ (root)`.
6. Нажми `Save`.

## Как менять древо

Открываешь `family.json` на GitHub → Edit → меняешь данные → Commit changes.

GitHub Pages опубликует новую версию после commit.
Открытая страница сама проверяет `family.json` каждые 30 секунд, поэтому после
публикации обновления F5 обычно не нужен.

Важно: публикация GitHub Pages не гарантированно мгновенная. GitHub указывает,
что после push изменения могут публиковаться до 10 минут.

## Добавить человека

В нужную группу:

```json
{
  "icon": "💜",
  "name": "Nickname",
  "role": "кем является"
}
```

Не забывай запятые между объектами JSON.
