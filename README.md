# Выпускной проект на платформе SkillFactory. Курс "Профессия Java-разработчик".

## Общая информация:
Проект представляет из себя API для Интернет-банка.
В проекте реализовано Rest API для получения из базы-данных информации о состоянии
счета клиента, пополнения счета клиента и списания с средств со счета клиента.

## Используемые технологии:
* Spring Boot v.3.0.0
* Spring Web v.3.0.0
* Spring Data v.3.0.0
* Lombok 
* Postgres DB v.14

## Реализованные функции:
В текущей версии реализованы 4 комнды в API:
1. getMoney(Long id) - получение информации о балансе клиента банка из БД по id клиента.
2. takeMoney(Long id, double money) - списание средств со счета клиента по id клиента, при условии, что баланс счета больше или равен сумме списания.
3. putMoney(Long id, double money) - зачисление средств на счет клиента по id клиента.
4. getAllClients() - получение информации из БД о состоянии счетов всех клиентов.

## Структура БД:
id - первичный ключ, id клиента
balance - колчиество денег не счету клиента

![image](https://user-images.githubusercontent.com/93705476/208083551-fb8be15e-149e-4cee-9342-dbeb3d7358e0.png)
