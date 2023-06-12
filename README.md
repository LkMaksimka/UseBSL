# Проверка кода
## Проверка код с помощью PhoenixBSL

### Установка
 1. Скачиваем с [phoenixbsl](https://github.com/otymko/phoenixbsl) файл [phoenixbsl-0.5.0-rc.1.msi](https://github.com/otymko/phoenixbsl/releases/download/v0.5.0-rc.1/phoenixbsl-0.5.0-rc.1.msi). 
 2. Скачиваем с [bsl-language-server](https://github.com/1c-syntax/bsl-language-server/releases) архив **[bsl-language-server_win.zip](https://github.com/1c-syntax/bsl-language-server/releases/download/v0.21.0-rc.2/bsl-language-server_win.zip)**
 3. В каталоге "С:\\Program Files\\phoenixbsl\\app\\" удаляем папку **bsl-language-server**
 4. Папку **bsl-language-server** из архива **bsl-language-server_win.zip** разпаковываем в каталог "С:\\Program Files\\phoenixbsl\\app\\"
 5. Запускаем **phoenixbsl.exe** из "С:\\Program Files\\phoenixbsl\\"

### Портативная версия
Скачиваем [сборку](https://github.com/LkMaksimka/UseBSL/releases), разпаковываем в любое место, запускаем **phoenixbsl.exe**, пользуемся.

### Выполнение проверки
#### [Диагностики](https://1c-syntax.github.io/bsl-language-server/diagnostics)
-   `CTRL` + `I` - анализ кода на замечания.
-   `CTRL` + `K` - форматирование кода.
-   `CTRL` + `J` - "исправить все в модуле" - автоматическое исправление определенных замечаний (см. "[Быстрые исправления](https://github.com/otymko/phoenixbsl#быстрые-исправления)").

### Пример настройки исключений
в файле "bsl-language-server.json"
``` bsl-language-server.json
{
    "language": "ru",
    "codeLens": {
        "showCognitiveComplexity": false,
        "showCyclomaticComplexity": false
    },
    "diagnostics": {
        "computeTrigger": "onSave",
        "skipSupport": "never",
        "parameters": {
            "Typo": {
                "minWordLength": 3,
                "userWordsToIgnore": "Разукомплектация,Разукомплектации,разукомплектации,Разукомплектацию"
			},
			"MissingParameterDescription": false
        }
    },
    "traceLog": null,
    "configurationRoot": "src"
}
}