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

![Desktop Screenshot 2024 11 06 - 16 50 47 21](https://github.com/user-attachments/assets/27110d12-4c05-4296-afee-5283a82e5d9e)

![Desktop Screenshot 2024 11 06 - 16 51 13 52](https://github.com/user-attachments/assets/6db803d1-50cc-47aa-9626-1971751e46dc)


  </details>

## Отчет по практической работе №4 

<details>
  <summary>Нажмите, чтобы развернуть</summary>

 Network Threat Hunting
 
## Скачиваем и разворачиваем стенд

![Desktop Screenshot 2024 12 01 - 13 55 34 31](https://github.com/user-attachments/assets/e267b5be-1451-4bb7-8861-452a4b9c7404)

Логинимся

![Desktop Screenshot 2024 12 01 - 14 07 57 32](https://github.com/user-attachments/assets/31c80cc9-1e0e-4c93-a9cb-0a357a326eab)

Добавляем адрес с траффиком к skype.com в safelist, как сказано в руководстве

![Desktop Screenshot 2024 12 01 - 14 07 21 30](https://github.com/user-attachments/assets/321e041c-d6e7-4681-9912-df570affe610)

![Desktop Screenshot 2024 12 01 - 14 22 23 47](https://github.com/user-attachments/assets/8d255d7e-51c5-446f-a4ae-1a38c6ccd560)

![Desktop Screenshot 2024 12 01 - 14 26 07 37](https://github.com/user-attachments/assets/489333d4-7015-4229-8dc4-be6c02b4e664)

Конечный safelist

![Desktop Screenshot 2024 12 01 - 14 26 54 21](https://github.com/user-attachments/assets/44c945e0-0824-47af-bd87-18842ddaf033)

## Lab 1

Импортируем логи и переключаемся на них в стенде

![Desktop Screenshot 2024 12 01 - 14 20 47 59](https://github.com/user-attachments/assets/5579f614-c139-4875-ae94-fd11dd4127ce)

Выбираем нужный Database

![Desktop Screenshot 2024 12 01 - 14 27 20 84](https://github.com/user-attachments/assets/6561c7c7-1af9-4ffb-b55b-f8bc68881cb7)

Переходим в модуль beacon web и анализируем 

![Desktop Screenshot 2024 12 01 - 14 29 00 65](https://github.com/user-attachments/assets/4a66736a-c065-4142-bba8-70c28c775f94)

![Desktop Screenshot 2024 12 01 - 14 30 02 85](https://github.com/user-attachments/assets/c3f7e125-18a6-475d-97cb-4201f63953cc)

Анализ всех адресов показал, что - 

Высокий уровень согласованности метрик (99.70%):

Такая высокая согласованность (cumulative metric conformity) может свидетельствовать о регулярных, четко упорядоченных запросах от источника к целевому IP-адресу. 
Это может быть признаком Beaconing-а, когда зараженное устройство связывается с управляющим сервером (C2).

Общее количество соединений (3011):

Для одного IP-адреса это значительное количество соединений. Если это типично для сети, возможно, это не аномалия. Но если такая активность не ожидается (например, для обычного пользователя или устройства IoT), это может указывать на нежелательное поведение.
Равномерное распределение активности на графике:

Использование HTTP без шифрования:

Отсутствие HTTPS может означать, что данные передаются в незашифрованном виде, что рискованно. Для связи с C2-серверами часто используются такие незащищенные протоколы.

Практически все адреса связаны с Windows, так что добавляем их в safelist

Конечный safelist

![Desktop Screenshot 2024 12 01 - 14 34 08 05](https://github.com/user-attachments/assets/c1f2f4d5-a732-4a37-939f-57b4d9262744)

Перейдём в модуль длительных соединений

![Desktop Screenshot 2024 12 01 - 14 35 56 73](https://github.com/user-attachments/assets/791cfa0e-62b0-4949-9427-5fb44ee70b23)

Всего 2 адресса, проверим их через VirusTotal

![Desktop Screenshot 2024 12 01 - 14 39 36 01](https://github.com/user-attachments/assets/75b12901-9f43-42b3-8d81-7bd90363fc86)

![Desktop Screenshot 2024 12 01 - 14 39 41 20](https://github.com/user-attachments/assets/dc133526-f8e2-4a37-b226-7788b7cde088)

VirusTotal пометил один из адресов, как вредоносный.

Подозрительная природа доменов
Связанные с IP домены `piensorcad6302755c.aiihosted.com` и `demo1.aiihosted.com` выглядят подозрительно:
Длинные, автоматически сгенерированные имена часто используются злоумышленниками для маскировки.
Домены связаны с поддоменами `aiihosted.com`, что может указывать на временную инфраструктуру (например, для фишинга, C2 или ботнетов).

Связь с DigitalOcean
Этот IP принадлежит хостинг-провайдеру `DigitalOcean`, который, как и другие публичные облачные провайдеры, часто используется для легальных целей. Однако злоумышленники также арендуют облачные серверы для вредоносной активности, таких как:
Развёртывание C2-серверов.
Проведение атак (например, DDoS, фишинг).

Связь с файлом `"7May2021_export_bookmark.html"`:
Хотя файл не был помечен как вредоносный, сама его природа (экспорт закладок) может намекать на использование IP для передачи данных, что требует дополнительного анализа.

## Lab 2

Импортируем логи и переключаемся на них.

![Desktop Screenshot 2024 12 01 - 14 39 41 20](https://github.com/user-attachments/assets/d7a92e5b-7ac0-49de-8355-8c2b80c6c2e8)

На основной странице пусто, но система отсылается к модулю DNS, убираем фильтры

![Desktop Screenshot 2024 12 01 - 14 45 40 51](https://github.com/user-attachments/assets/b78f6d15-d7eb-4eb9-9ea7-a7f144393d23)

Подозрительный домен: `honestimnotevil.com`
Название домена вызывает подозрения из-за своей провокационной природы ("честно, я не злой"), что может быть попыткой злоумышленников замаскировать свои намерения.
Такие имена доменов часто используют в тестовых или вредоносных инфраструктурах.

Большое количество запросов (2074 запросов)
Это аномальное количество DNS-запросов к одному домену, что может свидетельствовать о:
Подключении к Command & Control серверу.
Вредоносной программе, регулярно обращающейся к этому домену.

Длинные поддомены

Например:
`...b7f9090b8e40bac43eb80a.honestimnotevil.com`
`...291b4324545e080e82a0ea.honestimnotevil.com`

Длинные, случайно сгенерированные поддомены часто используются в доменной генерации (DGA — Domain Generation Algorithm), которая характерна для вредоносных программ.
Каждый новый поддомен может быть связан с уникальной сессией или устройством, участвующим в ботнете.

Связь с единственным хостом: `172.21.8.157`
Все запросы направлены на один IP-адрес (172.21.8.157).
Это может быть внутренний сервер или прокси для перенаправления запросов, но такой концентрации трафика стоит уделить внимание.

Нет прямых соединений (Direct Connections = 0)
Указано, что прямые соединения отсутствуют, что говорит о том, что злоумышленники могут использовать DNS-туннелирование для передачи данных через DNS-запросы.
Что меня смущает:
DNS-туннелирование или C2-активность

Количество запросов и странные поддомены сильно указывают на DNS-туннелирование или связь с Command & Control сервером.
DGA (Domain Generation Algorithm)

Автоматически сгенерированные поддомены и подозрительный основной домен усиливают вероятность того, что это вредоносная инфраструктура.
Аномальная активность в сети

Если это единственный хост (172.21.8.157), отправляющий такие запросы, он может быть скомпрометированным устройством.

## Lab 3 

![Desktop Screenshot 2024 12 01 - 14 46 27 68](https://github.com/user-attachments/assets/c1b48a56-a203-4651-9a9a-b7174f5ba605)

![Desktop Screenshot 2024 12 01 - 14 50 20 30](https://github.com/user-attachments/assets/4b941fb7-990a-4c1d-9ce0-306eb55b0e01)

Переходим в модуль beacons web

![Desktop Screenshot 2024 12 01 - 14 51 07 01](https://github.com/user-attachments/assets/66500f76-7a20-4ccf-ba29-45cf256b4f50)

Анализируем адреса и вносим легитивные в safelist

![Desktop Screenshot 2024 12 01 - 14 51 39 36](https://github.com/user-attachments/assets/a25e4442-edb6-4bc3-87df-fb20cd8d1033)

Остается всего два адреса, проверим каждый через VirusTotal

![Desktop Screenshot 2024 12 01 - 14 52 24 04](https://github.com/user-attachments/assets/6fe8e36a-4607-4eeb-b4c7-d80a0abe12f6)

Связь с вредоносной активностью

Метка DGA и упоминание Cobalt Strike усиливают подозрения, что домен используется для управления вредоносной активностью.
Количество детекций

Пять независимых сервисов отметили домен как вредоносный, что повышает вероятность его использования в атаках.
Неопределённость IP-адреса

`IP 210.71.232.11` необходимо анализировать отдельно. Если он используется несколькими подозрительными доменами, это усилит подозрения.
Свежесть данных

Анализ проводился месяц назад, что недостаточно актуально для оценки текущей активности домена.

</details>
