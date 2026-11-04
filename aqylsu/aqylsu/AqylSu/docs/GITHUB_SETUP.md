# Загрузка AqylSu на GitHub

## Данные для нового репозитория

| Поле | Готовое значение |
| --- | --- |
| Repository name | `aqylsu` |
| Description / About | `AqylSu — симулятор умного полива с 3D-камерой, управлением грядками, расписаниями и учётом воды. HTML, CSS, JavaScript.` |
| Topics | `smart-irrigation`, `agriculture`, `agritech`, `javascript`, `html`, `css`, `canvas`, `simulation`, `kazakhstan` |
| Первый commit | `Add AqylSu irrigation simulator and project documentation` |

## Через сайт GitHub

1. Распакуйте `AqylSu_GitHub.zip` и откройте папку `AqylSu`.
2. Создайте новый репозиторий с именем `aqylsu`. Для публичного демо на бесплатном тарифе выберите **Public**. README уже подготовлен в архиве.
3. В пустом репозитории нажмите **uploading an existing file**; в существующем — **Add file → Upload files**.
4. Перетащите **содержимое папки `AqylSu`** в область загрузки. Сохраните структуру `docs` и `.github`.
5. Укажите сообщение первого коммита из таблицы и сохраните изменения предложенной GitHub кнопкой. Если создан pull request, объедините его после проверки.
6. Убедитесь, что `index.html` и `README.md` находятся в корне репозитория. ZIP-файл не заменяет распакованные исходники.

Если при выборе файлов папки не сохраняются, используйте перетаскивание папок или загрузку через Git ниже.

## Через Git в Windows

Создайте **пустой** репозиторий `aqylsu`, затем откройте терминал в распакованной папке `AqylSu`. Замените `YOUR_USERNAME` своим логином GitHub:

```powershell
git init
git add .
git commit -m "Add AqylSu irrigation simulator and project documentation"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/aqylsu.git
git push -u origin main
```

Эти команды рассчитаны на новую папку без Git-истории и пустой удалённый репозиторий. Если Git просит имя и email, задайте свои данные коммитов по его подсказке. Авторизацию выполните стандартным способом GitHub.

## Включение сайта на GitHub Pages

1. Откройте **Settings → Pages** в репозитории.
2. В **Build and deployment → Source** выберите **Deploy from a branch**.
3. Выберите ветку **main** и папку **/(root)**.
4. Нажмите **Save** и дождитесь завершения публикации.
5. Скопируйте адрес, который GitHub покажет в разделе Pages, в поле **Website** блока **About**.

Для репозитория `aqylsu` адрес обычно имеет вид:

```text
https://YOUR_USERNAME.github.io/aqylsu/
```

Это шаблон адреса: действующую ссылку предоставляет GitHub после успешной публикации. При ошибке проверьте вкладку **Actions**, выбранную ветку и наличие `index.html` в корне. Условия доступности Pages зависят от тарифа и видимости репозитория.

## Перед демонстрацией

- Откройте опубликованный адрес и проверьте «Камера 3D» и запуск полива.
- При необходимости перенесите свою ферму через JSON-копию: у сайта и локального файла отдельные данные.
- При выборе условий распространения добавьте соответствующий файл `LICENSE`.
- Используйте [сценарий демонстрации](DEMO.md).

Официальные инструкции: [загрузка файлов](https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository) и [настройка GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).
