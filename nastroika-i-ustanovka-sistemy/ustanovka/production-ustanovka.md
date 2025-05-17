# Production установка

## Docker

{% hint style="warning" %}
Если до этого у вас не был установлен Docker, пожалуйста, установите. Без этого ничего работать не будет [\[Ссылка на гайд по установке\]](https://docs.docker.com/engine/install/)
{% endhint %}

### Настройте переменные окружения

Пример: [https://github.com/CodeBattles-nn/codebattles/blob/new\_backend/.env.example](https://github.com/CodeBattles-nn/codebattles/blob/new_backend/.env.example)\


{% code title=".env.example" lineNumbers="true" %}
```properties
DB_USER=dfvdsdfvsdswvdfvdsvdfvdf
DB_PASSWORD=dvnsevhjeiwurowuqvhjevfvuodfb
DB_NAME=cb

```
{% endcode %}

{% stepper %}
{% step %}
### Создайте файл .env

Структура назодится в .env.example
{% endstep %}

{% step %}
### Задать сложные настройки

В файле .env
{% endstep %}
{% endstepper %}

### Выберете вашу архитектуру

{% tabs %}
{% tab title="x64" %}
Для установки потребуется скачать репозиторий и развернуть Docker compose Container

скачивание образов из репозитория:

```bash
docker compose -f prod-docker-compose.yml pull
```

запуск:

```sh
docker compose -f prod-docker-compose.ymlup
```


{% endtab %}

{% tab title="другие" %}
Для установки потребуется скачать репозиторий и развернуть Docker compose Container

сборка образов:

```bash
docker compose -f prod-docker-compose.yml build
```

запуск:

```sh
docker compose -f prod-docker-compose.yml up
```
{% endtab %}
{% endtabs %}

{% hint style="info" %}
Для запуска контейнеров в фоновом режиме используйте флаг _<mark style="color:blue;">**-d**</mark>_

Пример:

{% code fullWidth="false" %}
```bash
docker compose up -f prod-docker-compose.yml -d
```
{% endcode %}
{% endhint %}

После этого, пожалуйста, настройке языки программирования. Это описано на следующей странице
