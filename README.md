# Проектная кухня

Так мы называем коллективную работу над проектом, проходящую параллельно с курсом по React в Яндекс.Практикуме. По желанию студенты делятся на команды и переделывают несложное приложение на React и Redux. Это закрепляет навыки кодинга и тренирует навыки коллективной работы.

## О проекте в этом репозитории

Здесь лежит бэкенд, который мы подготовили для удобного запуска проекта в Docker. Оригинальный код этого приложения можно посмотреть в [репозитории Real World бэкенда на Express](https://github.com/gothinkster/node-express-realworld-example-app). Если вам не нравится работать с Docker'ом, вы можете взять приложение оттуда и запустить локально, установив MongoDB. Инструкции по установке MongoDB попросите у наставника. Но мы рекомендуем использовать этот проект и Docker. Так проще будет опубликовать приложение в сети.



## Запуск

Перед запуском, вам нужно установить Docker себе на компьютер.[Скачать установщик Docker Desktop](https://www.docker.com/get-started).

После установки, проверьте, что Docker работает, набрав `docker` в терминале.

После установки Docker

1. Переместитесь в директорию приложения
2. `make run` — соберет и запустит сервис по адресу `localhost:3000`
3. `make stop` — остановит сервис
4. `make start` — если сервис однажды был собран, включит его, не пересобирая (это быстрее)

### Особенности Windows

Чтобы запустить этот бэкэнд на ОС Windows, может потребоваться установка `make`. 

Для этого:

В powershell с правами администратора устанавливаем `chocolatey` командой

```powershell
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
```

Ставим make

```powershell
choco install make
```

## Вопросы

Если возникли вопросы, пишите в slack, вам помогут.
