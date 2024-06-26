# Алгоритм роутинга и балансировки на уровне Messaging Grid

## Контекст:

Мы приняли решение о том, что распределением пользовательской нагрузки между юнитами системы будет заниматься компонент Messaging Grid. Его функции должны включать маршрутизацию и балансировку запросов.

Пользователи нашей системы находятся по всему миру, причем распределены неравномерно, а также распределение может меняться в случае проведения масштабных спортивных мероприятий или выхода компании на новые рынки. 

Одним из нефункциональных требований является сопоставимо быстрое время отклика во всех регионах, где приложение будет использоваться. Также требуется соблюдать законодательство стран, где мы работаем, а в ряде государств оно требует хранения пользовательских данных на их территории.

## Решение

Для распределения пользовательской нагрузки компонент Messaging Grid будет использовать GeoDNS с маршрутизацией запроса на основании местоположения пользователя, определяемого по его IP адресу.

## Статус:

принято

## Последствия:

1. Удастся снизить время ответа за счет направления запросов пользователя к географически ближайшему серверу.
2. Можно будет легко осуществлять масштабирование за счет добавления новых юнитов в тех регионах, где это требуется.
3. Выдача пользователям локализованного контента будет осуществляться более удобным образом.
4. Геолокационные данные IP адресов могут быть неточными или устаревшими, в результате запросы некоторых пользователей могут направляться по неоптимальным маршрутам.
5. В случае нахождения пользователя в "пограничной зоне" между территориями которые обрабатываются разными юнитам, его запросы могут направляться на разные юниты, особенно при смене IP адреса и использовании мобильных сетей.