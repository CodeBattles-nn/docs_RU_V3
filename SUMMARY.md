# Table of contents

* [О системе V3](README.md)

## Обзор

* [Интерфейс участника](obzor/interfeis-uchastnika.md)
* [Интерфейс учителя](obzor/interfeis-uchitelya.md)

## Установка

* [Установка](ustanovka/ustanovka.md)
* [Значения по умолчанию](ustanovka/znacheniya-po-umolchaniyu.md)
* [Как зайти](ustanovka/kak-zaiti.md)
* [Настройка языков программирования](ustanovka/nastroika-yazykov-programmirovaniya.md)
* [Образы чекеров](ustanovka/obrazy-chekerov.md)

## Как работает система

* [Архитектура](kak-rabotaet-sistema/arkhitektura.md)
* [Production Архитектура](kak-rabotaet-sistema/production-arkhitektura.md)

## Свое соревнование

* [Подготовка задач](svoe-sorevnovanie/podgotovka-zadach/README.md)
  * [Создание своей задачи](svoe-sorevnovanie/podgotovka-zadach/sozdanie-svoei-zadachi.md)
  * [Импорт готовой задачи](svoe-sorevnovanie/podgotovka-zadach/import-gotovoi-zadachi.md)
* [Создание соревнования](svoe-sorevnovanie/sozdanie-sorevnovaniya.md)

## Backend API

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
