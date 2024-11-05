# Scel Система для сбора событий и логов
 
## Отчет по практической работе №1

<details>
  <summary>Нажмите, чтобы развернуть</summary>

## Rsyslog. Сервер

1 На виртуальных машинах настроил сеть на Сетевой мост 

2 На первой виртуальной машине скачем rsyslog

![Desktop Screenshot 2024 09 11 - 18 30 32 61](https://github.com/user-attachments/assets/558a706d-9d84-43c2-b1f8-9c774f328ba0)

3 Запустим сервис. Проверим работоспособность

![Desktop Screenshot 2024 09 11 - 18 31 06 06](https://github.com/user-attachments/assets/e58326f6-e89c-4581-9381-a976c4e68f26)

4 Настраиваем rsyslog для удаленного приема системного журнала

![Desktop Screenshot 2024 09 11 - 18 33 09 92](https://github.com/user-attachments/assets/9bd65fcf-e82d-48d0-bb94-5b544c2dd993)

5 Перезапускаем сервис

![Desktop Screenshot 2024 09 11 - 18 34 28 10](https://github.com/user-attachments/assets/1c36b05e-40f1-4c90-9cd3-31f3b8359995)

## Rsyslog. Клиент

1 На второй виртуальной машине скачаем rsyslog


2 Отредактируем config, добавляем правило для пересылки логов

![Desktop Screenshot 2024 09 11 - 18 35 58 05](https://github.com/user-attachments/assets/1d1d7ff1-f377-4041-a061-50c5608c366c)

3 Перезапускаем сервис

![Desktop Screenshot 2024 09 11 - 18 36 30 76](https://github.com/user-attachments/assets/70a45ee8-fa3a-4307-ab95-f8bf7c2a093d)

## LOKI

1 Разворачиваем на сервере Loki

![Desktop Screenshot 2024 09 11 - 18 57 31 69](https://github.com/user-attachments/assets/ebd01baf-7ffc-4c90-8fd7-fc741e2aa96f)

2 На клиенте устанавлиеваем Promtail

![282036573-44c92d3b-1497-477d-9b9d-cd2aebf7feb1](https://github.com/user-attachments/assets/dec84b26-7519-4276-ad05-657aa4d9e40c)

3 Создаем файл конфинфигурации

![Desktop Screenshot 2024 09 11 - 18 57 09 38](https://github.com/user-attachments/assets/c604ba7a-5a47-48f9-b0b3-002b7c5aef8b)

4 Создаем Unit

![Desktop Screenshot 2024 09 11 - 18 58 39 93](https://github.com/user-attachments/assets/e8fe05da-ce48-450e-aee7-c07681df4232)

![Desktop Screenshot 2024 09 11 - 18 59 34 73](https://github.com/user-attachments/assets/3dd5a127-81b5-407b-a18f-bc84d52d126a)

5 Перезапускаем сервис

![Desktop Screenshot 2024 09 11 - 19 00 54 74](https://github.com/user-attachments/assets/040a46b4-afa4-46a6-ab89-d85f528272fe)

6 Посмотрим логи на сервере

![Desktop Screenshot 2024 09 11 - 19 12 34 04](https://github.com/user-attachments/assets/d58cc6b4-a0dd-4748-9834-6ad17440085a)

![Desktop Screenshot 2024 09 11 - 19 12 53 15](https://github.com/user-attachments/assets/f00ebef9-0633-4af8-9e98-af69ee776487)

## SIGNOZ

1 Запускаем контейнер на сервере

![Desktop Screenshot 2024 09 11 - 19 20 46 83](https://github.com/user-attachments/assets/79fe5bba-bb61-4c26-ad42-e92154b3abe9)

2 Так же для клиента редактируем docker-compose файл

![Desktop Screenshot 2024 09 11 - 19 22 54 66](https://github.com/user-attachments/assets/270c4051-e45f-47c0-bf79-e6be491ff862)

3 Запускаем контейнер 

![Desktop Screenshot 2024 09 25 - 14 47 51 23](https://github.com/user-attachments/assets/26590260-afef-46ba-8e58-fc838e823e63)

4 Наблюдаем логи в SigNoz

![Desktop Screenshot 2024 09 25 - 14 47 51 25](https://github.com/user-attachments/assets/311b9120-8f8c-488a-ba86-327b782560b3)


![Desktop Screenshot 2024 09 25 - 14 47 51 26](https://github.com/user-attachments/assets/ac96cf69-1261-40eb-bfcd-d35065074a5c)


</details>

## Отчет по практической работе №2

<details>
  <summary>Нажмите, чтобы развернуть</summary>
 
https://colab.research.google.com/drive/1i-UAwV851rVhOP3LJ6zvfTDJJMig8LkN?usp=sharing

https://github.com/hipster-x/Scel/blob/main/PR2_sssl.ipynb

</details>

## Отчет по практической работе №3

<details>
  <summary>Нажмите, чтобы развернуть</summary>

В данной практике я выбрал готовый вариант Wazuh Server

![Desktop Screenshot 2024 10 23 - 17 40 34 02](https://github.com/user-attachments/assets/2a02955f-8879-45e6-a3b7-6c44bfc639c3)

![Desktop Screenshot 2024 10 23 - 18 31 45 29](https://github.com/user-attachments/assets/b48dad7f-b686-405f-933b-23cc85298f4a)

Авторизация

![Desktop Screenshot 2024 10 23 - 18 32 10 64](https://github.com/user-attachments/assets/2a580f71-b37a-4aa9-b3b3-aa1e1936bba0)

Веб-интерфейс Wazuh

![Desktop Screenshot 2024 10 23 - 18 33 11 25](https://github.com/user-attachments/assets/6098b1cd-da2c-439b-b61a-529939eee464)

Теперь готовимся установить агент на другой ВМ

![Desktop Screenshot 2024 10 23 - 18 47 30 13](https://github.com/user-attachments/assets/33a10e40-7ef4-4efd-a41d-3e66535658ab)

![Desktop Screenshot 2024 10 23 - 18 57 29 49](https://github.com/user-attachments/assets/f0453f67-ddec-44ea-9b30-a75946da6757)

Разворачиваем агент на второй ВМ

![Desktop Screenshot 2024 10 23 - 20 30 44 32](https://github.com/user-attachments/assets/170e2e6f-0370-47a7-8945-8c67471857eb)

![Desktop Screenshot 2024 10 23 - 20 31 03 94](https://github.com/user-attachments/assets/c2517fa5-8087-4ca0-b3e3-12db90638c26)

После настройки убедились, что агент настроен. И доступна машина для мониторинга

![Desktop Screenshot 2024 10 23 - 20 31 51 17](https://github.com/user-attachments/assets/6b4c060b-4765-46f4-9e9b-56a8b6cc5c73)

![Desktop Screenshot 2024 10 23 - 20 31 59 68](https://github.com/user-attachments/assets/8e4696c6-c362-4193-90d6-abee60090a49)

Система имеет встроенный детектор уязвимостей

![Desktop Screenshot 2024 10 23 - 20 39 34 80](https://github.com/user-attachments/assets/26648dab-eff5-4006-b30e-a5545b1fbe06)

![Desktop Screenshot 2024 10 23 - 20 42 56 21](https://github.com/user-attachments/assets/3a3a7fd0-2278-45c5-b29b-48b9925d7f23)

![Desktop Screenshot 2024 10 23 - 20 48 44 38](https://github.com/user-attachments/assets/7ce77388-d981-495e-9ba6-c52b4e08819c)

![Desktop Screenshot 2024 10 23 - 20 49 01 80](https://github.com/user-attachments/assets/3e62f660-90f6-4534-b069-b87615dbe18b)

![Desktop Screenshot 2024 10 23 - 20 49 09 98](https://github.com/user-attachments/assets/731fc465-0a4c-4fdd-bca2-c175e822da71)

Создание проверки целостности файлов

![Desktop Screenshot 2024 11 05 - 11 05 31 89](https://github.com/user-attachments/assets/c2eff684-47ca-40ef-a731-241c28e33292)

Настройка выявлений уязвимостей в соответствии с документацией

![Desktop Screenshot 2024 11 05 - 11 18 40 89](https://github.com/user-attachments/assets/d488c79e-037a-46d5-a3bf-a8196dd606ea)

Выявление скрытых процессов

![Desktop Screenshot 2024 11 05 - 11 11 38 20](https://github.com/user-attachments/assets/f145f3f0-b26f-456d-bcc6-c1a903d6506d)

Выявление SQL-инъекций

![Desktop Screenshot 2024 11 05 - 11 20 39 56](https://github.com/user-attachments/assets/5e9046b5-b2d2-49c3-b5ba-329dace39e7f)

Проверка работы настроенных механизмов

SQL injection

![Desktop Screenshot 2024 11 05 - 21 59 22 15](https://github.com/user-attachments/assets/6a2871de-a09f-4951-b0ef-1a2ccc75933e)

  </details>
