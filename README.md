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
