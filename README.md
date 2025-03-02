# КруБИС

## Сборка и запуск

```bash
npm install
```

Далее - стандартная сборка webpack, dev и prod режимы на данный момент ничем не отличаются. Файлы собираются в папку dist.

Для запуска достаточно любого статического сервера + прокси-сервера на https://krubiss.ru/api (нужен для обхода CORS и проблем с сертификатом у сайта). В качестве последнего можно использовать caddy, готовый конфиг уже присутствует.

## Интеграция на сайт

Для соответствия сайту с него были скопированы стили и помещены в файл `site-globals.css` - соответственно, при сборке для сайта этот файл нужно исключить (элегантного решения не реализовано, по-простому можно убрать импорт из `index.ts`).