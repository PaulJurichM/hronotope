# Общий хронотоп Бориса Акунина

Интерактивный исследовательский атлас художественного корпуса Бориса Акунина.

## Содержимое

- `index.html` — автономная интерактивная временная карта;
- `data/akunin_chronotope_all_v0_1.json` — исходная база временных карточек;
- `research/akunin_chronotope_research_v0_1.xlsx` — исследовательская таблица, методика и очередь проверки;
- `.nojekyll` — отключает обработку Jekyll для GitHub Pages;
- `publish-to-github.ps1` — безопасный загрузчик файлов в существующий репозиторий GitHub.

## Локальный просмотр

Откройте `index.html` в современном браузере.

## Публикация

1. Создайте пустой репозиторий на GitHub или выберите существующий.
2. Создайте fine-grained personal access token только для этого репозитория.
3. Разрешите токену доступ **Contents: Read and write**.
4. Запустите PowerShell в папке пакета:

```powershell
Set-ExecutionPolicy -Scope Process Bypass
.\publish-to-github.ps1
```

5. Введите `owner/repository`, ветку и PAT по запросу.
6. Для GitHub Pages откройте в репозитории **Settings → Pages**, выберите **Deploy from a branch**, нужную ветку и каталог `/ (root)`.

Токен вводится скрыто и не сохраняется в файлах или remote URL.
