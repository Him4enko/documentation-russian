# Процесс обновления
<!-- position: 4 -->

<h2 id="upgrade-from-major-version">Обновление с основной версии Bludit</h2>

Привиденные действия подходят для обновления основной версии Bludit. Основная версия - первая цифра в версии Bludit, например `Bludit v3.x`.

1. Выполните бэкап всей дериктории в которой находится Bludit.
2. Запомните или сделайте пометку версии установленного Bludit (Для возможного отката действий.)
3. Скачайте последнюю версию с [официального сайта](https://www.bludit.com).
4. Разархивируйте архив.
5. Загрузите разархивированные файлы к себе на хостинг с заменой файлов.
6. Очистите кэш вашего браузера. (В настройках браузера)
7. Войдите в админ-панель и проверьте настройки Bludit.
8. Готово.

> Примечание: Если ваш сайт кеширует каким-либо сервисом(Например: Cloudflare), то вам нужно очистить кеш в сервисе, который вы используете.

---

<h2 id="upgrade-from-bludit-2-to-bludit-3">Обновление Bludit с версии v2.3.4 до Bludit v3.0</h2>

Для обновления основных версий, рекомендуем использовать инструмент, созданный - [@anaggh](https://github.com/anaggh). Пожалуйста, ознакомьтесь с инструкций изложенной ниже, а также инструкцией в официальном репозитории инструмента.Если у вас возникли какие-либо трудности, вы можете задать свой вопрос на [форуме](https://forum.bludit.org) или в [онлайн чате](https://gitter.im/bludit/support).

### Инструкци до обновления основых версий.

- Выполните бэкап всей дериктории в которой находится Bludit (Абсолютно всей, а не некоторых папок и файлов).
- Плагины `Backups` и `Timemachine X` будут удалены вместе с содержимым.
- Инструмен обновления создат папку с именем `/migrations/` и внутри папку с именем `bl-content` в которой хранятся все данные совместимые с Bludit v3.0.
- После завершения обновления, вам нужно удалить все папки в каталоге, кроме папки - `/migrations/` и установить новую версию Bludit.
- После обновления, скопируйте папку (`bl-content`), которая находится по адресу`/migrations/bl-content` в ваш каталог, где расположена новая версия Bludit.

https://github.com/anaggh/bludit-scripts/tree/master/migration-v2-to-v3