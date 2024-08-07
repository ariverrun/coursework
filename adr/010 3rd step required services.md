# Выделение сервисов, необходимых на третьем этапе

## Контекст:

Мы реализовали функционал позволяющий пользователю заказывать товары, собирать из них инвентарь и использовать его для планирования тренировок. 

На третьем этапе нужно разработать систему достижений, добавить геймификацию, использование баллов за достижения в качестве бонусов согласно системе лояльности, а также проинтегрировать систему с социальными сетями.

Необходимо обозначить границы сервисов, которые будут выполнять все вышеперечисленные функции.

## Решение

Мы реализуем следующие сервисы:

1. Сервис достижений (Achievements), который регистрирует достижение пользователя по результатам сбора его метрик и уведомляет о нем пользователя.
2. Сервис системы лояльности (Loyalty), которая получает уведомление о достижении и начисляет бонусы согласно стратегии поощрения.
3. Сервис социальных сетей (Social Networks), который служит прослойкой между системой и социальными сетями и реализует функционал, позволяющий делать посты в них о новых достижениях.

Все эти сервисы будут объединены в рамках Process Unit.

![Сервисы третьего этапа](https://raw.githubusercontent.com/ariverrun/coursework/main/assets/010%203rd%20step%20required%20services.png "Сервисы третьего этапа")

## Статус:

принято

## Последствия

1. Разделение на сервисы позволит их независимо масштабировать, что важно, так как они будут иметь различную нагрузку.
2. Разделение на сервисы позволит их независимо разрабатывать.