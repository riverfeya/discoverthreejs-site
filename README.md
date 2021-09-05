# Добро пожаловать в Discover three.js!

Это публичный реппозиторий книги [Discover three.js](https://discoverthreejs.com/).

Пулл реквесты приветствуются, особенно для:

* Своевременного обновления книги новыми выпусками three.js.
* Исправлений в тексте или примерах кода.
* Любых других ошибок, проблемм с браузером или CSS..

Поищите в папке markdown слово "TODO", если вы ищете вдохновение. ^_^

Если вы хотите внести более крупный вклад, пожалуйста, свяжитесь с нами, прежде чем вносить изменения.

## Гайд разработчика

Вот процесс создания и просмотра книги.

Предпосылки: Node.js, [Hugo](https://github.com/gohugoio/hugo)

1. Клонируйте или скачайте реппозиторий
2. Скачайте Hugo _extended_ binary для свойе системы [here](https://github.com/gohugoio/hugo/releases) и поместите его в корне проекта. Протестировано с Hugo V0.82.1.
2. Выполните `npm install`
4. Выполните `npm start`
5. Перейдите на `http://localhost:1313/` чтобы цвидеть сайт. Возможно, вам потребуется убедиться, что этот порт открыт в вашем брандмауэре.

## Технические детали

Книга собрана на Hugo, и это репо следует довольно типичной структуре папок для проекта Hugo, хотя папка `content /` была переименована в `markdown /`.

### Важные папки

* `markdown` - все слова книги содержатся здесь.
* `assets/src` - исходный код JS.
* `assets/scss` - SCSS стили для книги.
* `static` - все статические файлы такие как картинки, шрифты, модели, текстуры, изображения, и favicons.
* `static/examples` - код для примеров IDE находится здесь. Каждый пример - это  `World` - например: `static/examples/worlds/first-steps/first-scene` содержит пример для главы **First Scene**. См. `static/examples/README.md`.
* `/public` - сюда будут помещены файлы, созданные Hugo с помощью команды `npm run production`. По умолчанию при разработке Hugo отображает файлы в памяти, однако может быть полезно сгенерировать файлы, если вам нужно их изучить.

## Notes

* [Hugo Pipes](https://gohugo.io/hugo-pipes/) are used to build [SCSS](https://gohugo.io/hugo-pipes/scss-sass/) and [JS](https://gohugo.io/hugo-pipes/js/) assets. This means the Hugo extended version must be used.
* Running `npm start` will take several seconds to bundle all the files so please be patient. However, once the server is running, updates should take just a few milliseconds.
