# Домашнее задание «Teamcity»

## Ссылка на репозиторий:
https://github.com/kandroid83/example-teamcity

## Что было сделано:
1. Развернута инфраструктура в Docker (TeamCity Server, Agent, Nexus).
2. Настроена интеграция с Maven и Nexus (settings.xml).
3. Настроены условия выполнения сборки: для ветки master — `mvn clean deploy`, для остальных — `mvn clean test`.
4. Конфигурация сборки мигрирована в репозиторий (Kotlin DSL).
5. Создана ветка `feature/add_reply`, в класс `Welcomer` добавлен метод `getHunterReply`, написан тест.
6. Ветка `feature/add_reply` слита в `master`.
7. Настроена публикация артефактов (`.jar`), сборка по `master` проходит успешно.
