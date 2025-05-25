# Table of contents

* [О системе V3](README.md)

## Обзор

* [Интерфейс участника](obzor/interfeis-uchastnika.md)
* [Интерфейс администратора](obzor/interfeis-administratora/README.md)
  * [Задачи](obzor/interfeis-administratora/zadachi.md)
  * [Чекеры](obzor/interfeis-administratora/chekery.md)
  * [Соревнования](obzor/interfeis-administratora/sorevnovaniya.md)

## Настройка и установка системы

* [Установка](nastroika-i-ustanovka-sistemy/ustanovka/README.md)
  * [Локальная установка](nastroika-i-ustanovka-sistemy/ustanovka/lokalnaya-ustanovka.md)
  * [Production установка](nastroika-i-ustanovka-sistemy/ustanovka/production-ustanovka.md)

## Первое соревнование

* [Создать соревнование](pervoe-sorevnovanie/sozdat-sorevnovanie.md)

## Инструкции

* [Соревнование](instrukcii/sorevnovanie/README.md)
  * [Создание соревнования](instrukcii/sorevnovanie/sozdanie-sorevnovaniya.md)
  * [Редактирование чекеров соревнования](instrukcii/sorevnovanie/redaktirovanie-chekerov-sorevnovaniya.md)
  * [Редактирование пользователей соревнования](instrukcii/sorevnovanie/redaktirovanie-polzovatelei-sorevnovaniya.md)
  * [Редактирование задач соревнования](instrukcii/sorevnovanie/redaktirovanie-zadach-sorevnovaniya.md)
* [Задачи](instrukcii/zadachi/README.md)
  * [Добавить задачу](instrukcii/zadachi/dobavit-zadachu.md)
  * [Изменить задачу](instrukcii/zadachi/izmenit-zadachu.md)
  * [Удалить задачу](instrukcii/zadachi/udalit-zadachu.md)
* [Пользователи](instrukcii/polzovateli/README.md)
  * [Регистрация пользователей](instrukcii/polzovateli/registraciya-polzovatelei.md)
* [Чекеры](instrukcii/chekery/README.md)
  * [Создание чекера](instrukcii/chekery/sozdanie-chekera.md)
  * [Изменение чекера](instrukcii/chekery/izmenenie-chekera.md)
  * [Удаление чекера](instrukcii/chekery/udalenie-chekera.md)

## Как работает система

* [Архитектура](kak-rabotaet-sistema/arkhitektura.md)
* [Безопасность](kak-rabotaet-sistema/bezopasnost.md)

## API

* [Введение в API](api/vvedenie-v-api.md)
* [Backend](api/backend/README.md)
  * ```yaml
    type: builtin:openapi
    props:
      models: true
    dependencies:
      spec:
        ref:
          kind: openapi
          spec: doctorixx-api
    ```
* [Checker API](api/checker-api/README.md)
  * ```yaml
    type: builtin:openapi
    props:
      models: false
    dependencies:
      spec:
        ref:
          kind: openapi
          spec: codebattles-checker-api
    ```
