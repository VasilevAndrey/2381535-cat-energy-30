# Личный проект «Кэт энерджи»

[![Project check][check-image]][check-url]

* Студент: [Андрей Васильев](https://up.htmlacademy.ru/adaptive/30/user/2381535).
* Наставник: [Сергей Артёмов](https://htmlacademy.ru/profile/firefoxic).

---

В корне проекта находятся только его конфиги. А также полезные файлы:

* [Contributing.md](Contributing.md) — руководство по внесению изменений.
* [Workfolw.md](Workfolw.md) — описание структуры проекта и работы с ним.

**Исходные файлы вёрстки должны лежать в `source/`.**

Собирается проект в `build/`.

---

## Установка зависимостей проекта

Сложная сборка в этом проекте не заведётся без дополнительных инструментов — зависимостей. Поэтому их необходимо установить.

### 1. Терминал

Для установки зависимостей понадобится терминал. В Linux и macOS он уже есть, а в Windows надо установить _git-bash_, который идёт в комплекте с самим [Git](https://git-scm.com/download/windows).

### 2. Node.js

Зависимости работают в среде _node.js_, которую тоже нужно установить, но лучше не с помощью установщика с официального сайта, а через менеджер версий ноды — _nvm_. Для его установки выполни в терминале:

```shell
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.5/install.sh | bash
```

Перезапусти терминал и убедись, что _nvm_ работает:

```shell
nvm -v
```

Команда должна вывести версию _nvm_ — `0.39.5`. Если отвечает, что команда не найдена, то надо выполнить эту команду:

```shell
echo 'export NVM_DIR="$HOME/.nvm"' >> ~/.profile && echo '[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"' >> ~/.profile
```

И снова перезапусти терминал и проверь версию _nvm_. Когда выведет её, можно установить сам _node.js_:

```shell
nvm install --lts --default
```

После этого выполни:

```shell
node -v
```

Команда должна вывести версию _node.js_, например `v20.10.0`, что означает успешность установки.

### 3. Зависимости

Вместе с нодой стал доступен её менеджер пакетов _npm_. Но в проекте используется его альтернатива — _pnpm_. Он по умолчанию отключён, надо включить командой:

```shell
corepack enable
```

После этого для установки зависимостей проекта в терминале, находясь в директории проекта, выполни:[^1]

```shell
pnpm i
```

[^1]: **Не** обращай внимание на предупреждения во время установки.

### 4. Работа с проектом

После установки зависимостей становится доступным любой pnpm-скрипт проекта. Все доступные скрипты можно посмотреть выполнив:

```shell
pnpm run
```

Но для начала достаточно запомнить эти два наиболее часто используемые:

1. Линтинг — последовательная проверка кода пятью линтерами:

    ```shell
    pnpm lint
    ```

2. Cборка для разработки, при которой запустится и локальный сервер в папке `build/`, в которую собирается проект из папки `source/`, а в брауезере откроется разрабатываемый сайт и будет обновляться при обновлении файлов в проекте:

    ```shell
    pnpm start
    ```

Больше подробностей про использование команд можно найти в [Workfolw.md](Workfolw.md).

---

<a href="https://htmlacademy.ru/intensive/adaptive"><img align="left" width="50" height="50" alt="HTML Academy" src="https://up.htmlacademy.ru/static/img/intensive/adaptive/logo-for-github-2.png"></a>

Репозиторий создан для обучения на профессиональном онлайн‑курсе «[HTML и CSS. Адаптивная вёрстка и автоматизация](https://htmlacademy.ru/intensive/adaptive)» от [HTML Academy](https://htmlacademy.ru).

[check-image]: https://github.com/htmlacademy-adaptive/2381535-cat-energy-30/workflows/Project%20check/badge.svg?branch=master
[check-url]: https://github.com/htmlacademy-adaptive/2381535-cat-energy-30/actions
