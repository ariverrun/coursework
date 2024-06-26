# Архитектурный подход к MVP

## Контекст:

Мы реализуем MVP и нам нужно выбрать, в каком стиле он будет реализован. Ранее, на этапе анализа требований и составления плана разработки мы выбрали Space-based подход, как наиболее подходящий для выполнения поставленной задачи. 

Space-based архитектура была выбрана как хорошо поддающаяся масштабированию, легко локализуемая и позволяющая сделать систему высоко производительной. На первом этапе разработки MVP эти характеристики также являются необходимыми.

У компании уже есть используемые продукты и новая система не должна выдерживать ту нагрузку, которую создадут пользователи переходя на нее со старых приложений.

Опции:

1. Реализовать MVP в виде монолита.
2. Реализовать MVP с использованием сервисного подхода.
3. Реализовать MVP сразу создавая Space-based архитектуру.

Монолит позволит реализовать MVP в кратчайшие сроки, но система должна хорошо поддерживать географическую распределенность и обслуживать большое количество клиентов уже на начальном этапе. Сервисный подход не решит этой проблемы. Space-based архитектура позволит уже на этапе MVP выполнить эти требования, без которых MVP строго говоря и не MVP, потому что не сможет отвечать минимальным требованиям доступности.

## Решение

Мы реализуем Space-based подход с самого начала.

## Статус:

принято

## Последствия:

1. Система с самого начала будет высокодоступной во всех географических точках, где это требуется.
2. Система с самого начала сможет справляться с большим количеством пользователей.
3. Потребуется больше времени на реализацию MVP.