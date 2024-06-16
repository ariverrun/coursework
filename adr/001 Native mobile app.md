# Выбор платформы мобильного приложения

## Контекст:

Мы разрабатываем мобильное приложение, которое должно обладать богатым и отзывчивым интерфейсом, быть расширяемым и безопасным, интегрироваться со множеством различных датчиков, используемых спортсменами. У нас уже есть несколько мобильных приложений, функции которых должны быть перенесены в новое, которое мы собираемся реализовать. Эти приложения написаны с использованием разных технологий.

Опции:

1. Нативное мобильное-приложение, реализуемое с использованием Kotlin, Java, Swift.
2. Кроссплатформенное мобильное-приложение, реализуемое на базе фреймворков Flutter или React Native.

Нативные приложения:

1. Плюсы:
    1. Более высокая производительность и скорость.
    2. Прямой доступ к аппаратным функциям устройства и API операционной системы.
    3. Больше свободы при реализации уникальных интерфейсов.
    4. Проще реализовать требования к безопасности приложения.
2. Минусы:
    1. Выше стоимость разработки и обслуживания.
    2. Необходимость писать свой код под каждую платформу, с использованием разных языков, что исключает возможность переиспользования кода.

Кроссплатформенные приложения:

1. Плюсы:
    1. Один и тот же код работает на всех платформах.
    2. Ниже стоимость разработки.
    3. Выше скорость реализации.
2. Минусы:
    1. Меньшая скорость и производительность приложения.
    2. Меньше возможностей в реализации уникальных интерфейсов.
    3. Сложности с интеграцией сторонних устройств.
    4. Отсутствие доступа к нативным функциям устройства.

## Решение:

Мы реализуем нативное мобильное приложение. Версия под Android реализуется на Kotlin, под iOS на Swift.

## Статус:

принято

## Последствия:

1. В нативном приложении получится реализовать гибкий и богатый UI, сделать его отзывчивым для пользователя.
2. Удастся в полной мере использовать фитнес-функции смартфона.
3. Удастся интегрировать большее количество сторонних датчиков.
4. Приложение будет более безопасным.
5. Придется затратить больше времени на написание и поддержку кода.
6. Придется разрабатывать и поддерживать одновременно два приложения: под Android и под iOS.
7. Повышается вероятность того, что в результате ошибок могут появиться различия в работе приложения на разных платформах.
8. Разработка будет дороже в силу того, что потребуется больше разработчиков и с более высокой компетенцией.
