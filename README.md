# Проверка кода
## Проверка код с помощью PhoenixBSL

 1. Скачиваем с github [phoenixbsl](https://github.com/otymko/phoenixbsl)  файл [phoenixbsl-0.5.0-rc.1.msi](https://github.com/otymko/phoenixbsl/releases/download/v0.5.0-rc.1/phoenixbsl-0.5.0-rc.1.msi), портативной версии на сайте нет,  поэтому ставим себе на комп и просто копируем папку. 
 2. Скачиваем с github [bsl-language-server](https://github.com/1c-syntax/bsl-language-server/releases) архив **[bsl-language-server_win.zip](https://github.com/LkMaksimka/UseBSL/releases/tag/PhoenixBSL_v0_5_0_rc_1_BSL_v0_21_0_ra_9)**
 3. В каталоге "С:\\Program Files\\phoenixbsl\\app\\" удаляем папку **bsl-language-server**
 4. Распаковываем архив **bsl-language-server_win** и папку  **bsl-language-server** копируем, в каталог "С:\\Program Files\\phoenixbsl\\app\\"
 5. Запускаем **phoenixbsl.exe** из "С:\\Program Files\\phoenixbsl\\"

### Выполнение проверки
#### [Диагностики](https://1c-syntax.github.io/bsl-language-server/diagnostics)
-   `CTRL` + `I` - анализ кода на замечания.
-   `CTRL` + `K` - форматирование кода.
-   `CTRL` + `J` - "исправить все в модуле" - автоматическое исправление определенных замечаний (см. "[Быстрые исправления](https://github.com/otymko/phoenixbsl#быстрые-исправления)").

### Сборка
[Готовая сборка](https://github.com/LkMaksimka/UseBSL/releases)
