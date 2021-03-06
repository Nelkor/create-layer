# Слой frontend

Родительским слоем является
[code](https://github.com/Nelkor/create-layer/blob/main/src/layers/code/readme/ru.md).

## Функциональность

### Sass (SCSS)

Мы можем создавать файлы `.sass`/`.scss` в директории `src` и писать стили
на языках Sass/SCSS.

Импорты алиасов, добавленных в `tsconfig.json`, работают по правилам Sass —
через символ `~`. Например:

```scss
@import '~@/style/ui';
```

### Webpack

Мы можем собрать проект для его доставки на сервер, а также запустить локальный
сервер разработки, подхватывающий изменения в проекте на лету.

По умолчанию, мы можем использовать в своих файлах с кодом и стилями
изображения в форматах:
* jpg
* png
* webp
* svg

А также шрифты в формате `woff2`.

### Декларации

Вышеперечисленные форматы изображений добавлены в файл `index.d.ts` в корне
проекта. Это значит, что анализатор TypeScript не будет против того, что мы
импортируем файлы с такими расширениями в свой код.

## Команды

* `npm run build` — соберёт проект.
* `npm run serve` — запустит dev-server (порт 5445).
* `npm run format-scss` — исправит ошибки форматирования в `.scss`-файлах.
