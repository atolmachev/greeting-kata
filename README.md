# The Greeting Kata

Эта [Kata](https://en.wikipedia.org/wiki/Kata_(programming)) пригодится чтобы попрактиковаться в написании тестов для чистых функций. Она специально начинается очень просто, постепенно усложняясь.

Эта Ката предложена [Nick Gauthier](http://ngauthier.com) и вдохновлена Бобом из [Exercism](http://exercism.io).

Эта Ката сделана для практики [[Detroit-school TDD]].

## Требование 1

Напишите метод `greet(name)` который интерполирует `name` в простое приветствие. Например, когда `name` = `"Вася"`, метод должен вернуть `"Привет, Вася."`.

## Требование 2

Обработайте null введя подмену. Например, когда `name` = null, метод должен вернуть `"Привет, мой друг."`

## Требование 3

Обработайте "кричащие" имена. Когда `name` записано заглавными буквами, метод должен "прокричать". Например, когда `name` = `"ВАСИЛИЙ"` метод должен вернуть `"ПРИВЕТ ВАСИЛИЙ!"`

## Требование 4

Обработайте два аргумента. Когда `name` - это два аргумента (varargs), оба имени должны быть распечататны. Например, когда `name` = `["Вася", "Санек"]`, метод должен вернуть `"Привет, Вася и Санек."`

## Требование 5

Обработайте любое число имен. Когда `name` содержит более двух имен, разделите их точкой, а последний разделитель будет "и". Например, когда `name` = `["Оля", "Ваня", "Катя"]`, метод должен вернуть строку `"Привет, Оля, Ваня и Катя."`

## Требование 6

Обработайте обычные имена и кричащие имена разделением на два приветствия. Например, когда `name` = `["Оля", "ИВАН", "Катя"]`, метод должен вернуть строку `"Привет, Оля и Катя. И ПРИВЕТ ИВАН!"`

## Требование 7

Если `name` содержит запятую, разделите его. Например, если `name` = `["Оля", "Катя, Ваня"]`, метод должен вернуть строку `"Привет, Оля, Катя, и Ваня."`.

## Требование 8

Разрешите эскейпинг запятых из Требования 7. Эскейпинг такой же как в файлах CSV, с двойными ковычками, окружающими вхождение. Например, когда `name` = `["Иван", "\"Люся, Агафья\""]`, метод должен вернуть строчку `"Привет, Иван и Люся, Агафья."`.