# Домашнее задание 1, Мостачев Андрей, БПИ197

## Функциональные требования (общие)

1. Регистрация и вход
2. Заполнение и изменение информации пользователя
3. Добавление и изменение способов оплаты
4. Использование функционала продавца и покупателя в рамках одного пользователя
5. Оставление отзывов о пользователях
6. Изменение данных авторизации

## Роли и действия пользователей

### Продавец

1. Создание аукциона
2. Заполнение информации о предмете аукциона
3. Закрытие аукциона
4. Оставление отзыва о покупателе
5. Получение уведомлений о ходе аукциона

### Покупатель

1. Поиск аукционов по названию/категории/времени
2. Ставка в аукционе
3. Оплата покупки
4. Оставление отзыва о продавце
5. Получение уведомлений о ходе аукциона

## Объекты

### Пользователь
1. ID
2. Имя пользователя
3. Данные аутентификации
4. Контактные данные
    1. Email
    2. Телефон
5. Платежные данные
    1. Банковская карта
    2. Телефон (может быть отличным от контактного)
    3. PayPal
7. Отзывы о пользователе
8. Аукционы
    1. Текущие аукционы
    2. История аукционов

### Банковская карта

1. ID
2. Номер
3. Владелец
4. Срок действия

### Аукцион

1. ID
2. Название
3. Срок
4. Описание
5. Начальная цена
6. Продавец
7. Ставки
8. Категория

### Ставка

1. ID
2. Пользователь
3. Аукцион
4. Сумма

### Отзыв

1. Автор
2. Объект отзыва
3. Текст
4. Оценка

## Связи между объектами

### Один к одному

1. Пользователь - банковская карта

### Один к многим

1. Пользователь - аукцион
2. Пользователь - отзыв
3. Аукцион - ставка
4. Пользователь - ставка

## Схема модели

https://drawsql.app/hse-19/diagrams/hw1