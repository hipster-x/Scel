# Практическая работа №5 Threat Hunting

Выполнил студент ББМО-02-23 Евдокимов А.М.

## Стенд

Для выполнения работы использовал стенд из практической работы 3

Стенд состоит из 3 виртуальных машин

1. Ubuntu с агентом Wazuh
2. Ubuntu с сервером Wazuh
3. Kali Linux

Готовый веб-интерфейс с подключенным wazuh - агентом

![Desktop Screenshot 2024 12 02 - 17 16 25 75](https://github.com/user-attachments/assets/a6e0a2da-2c1c-4bcc-a93a-c197cff02b6a)

## IDS Suricata

Развернем IDS Suricata на агенте

![Desktop Screenshot 2024 12 02 - 17 22 10 49](https://github.com/user-attachments/assets/2c510a76-3d2a-4a14-8973-9a6775c58ee7)

![Desktop Screenshot 2024 12 02 - 17 22 45 96](https://github.com/user-attachments/assets/e12d8260-5da0-4dbe-a7b8-f43198b06781)

Настраиваем конфигурацию

![Desktop Screenshot 2024 12 02 - 17 27 04 42](https://github.com/user-attachments/assets/62102ece-a97a-4009-bfd9-a5f6b5bb7556)

![Desktop Screenshot 2024 12 02 - 17 40 25 26](https://github.com/user-attachments/assets/b0446046-b47c-453f-a317-d78379c84807)

![Desktop Screenshot 2024 12 02 - 20 22 40 38](https://github.com/user-attachments/assets/0997d473-217b-47d9-be55-bd6b905e09d4)

Так же настроим сбор логов

![Desktop Screenshot 2024 12 02 - 17 33 17 75](https://github.com/user-attachments/assets/dd990f95-418c-427c-b4f7-f40e8046c57e)

И получаем логи Suricata

![Desktop Screenshot 2024 12 02 - 20 21 52 22](https://github.com/user-attachments/assets/af9dd82a-11fb-43e7-ba6c-415cb4f71514)

## Сканер уязвимостей Nikto

На агенте пустой Apache

![Desktop Screenshot 2024 12 02 - 20 23 28 24](https://github.com/user-attachments/assets/de87838f-8ce3-4830-9eaa-1363fe8be671)

Запускаем сканер уязвимостей

![Desktop Screenshot 2024 12 02 - 20 24 14 38](https://github.com/user-attachments/assets/c3a82357-2ac6-4c90-93cb-206e027d30ec)

Ловим события от Suricata

![Desktop Screenshot 2024 12 02 - 23 51 44 27](https://github.com/user-attachments/assets/27accc43-4cfb-48e2-a74e-f0ffff0ee0c4)

Подробнее

![Desktop Screenshot 2024 12 02 - 23 50 55 84](https://github.com/user-attachments/assets/4e3a4c0a-b097-4b9b-86d5-99e788f215fa)

![Desktop Screenshot 2024 12 02 - 23 51 05 10](https://github.com/user-attachments/assets/5b085c35-7797-4f27-9855-74e3c4da46bb)

![Desktop Screenshot 2024 12 02 - 23 51 13 77](https://github.com/user-attachments/assets/71c5f4de-f9ee-41bd-b7ef-1f3412469ea1)

## YARA 

### Агент

Скачиваем и устанавливаем yara, докачивая правила 

![Desktop Screenshot 2024 12 03 - 16 13 28 97](https://github.com/user-attachments/assets/290ef9f6-29ca-4508-910c-3fd49270f45d)

Создаем конфиг

![Desktop Screenshot 2024 12 03 - 00 37 17 08](https://github.com/user-attachments/assets/bb7d6304-6a5a-44a3-999e-e3689be29f76)

Редактируем ossec 

![Desktop Screenshot 2024 12 03 - 00 41 21 38](https://github.com/user-attachments/assets/23044af3-3c2d-4d6a-a45f-6501a6f012e4)

### Сервер

![Desktop Screenshot 2024 12 03 - 00 43 35 40](https://github.com/user-attachments/assets/a143a57b-6978-47f9-80f1-073904020bd0)

![Desktop Screenshot 2024 12 03 - 00 46 53 30](https://github.com/user-attachments/assets/d69184a0-75e7-4252-bdf3-5a010bffff6a)

На данном этапе я словил критическую ошибку на агенте и не смог работать на нем, поэтому пришлось преустановить на другую ВМ (далее ip `192.168.43.182`)

![Desktop Screenshot 2024 12 03 - 15 24 01 69](https://github.com/user-attachments/assets/f90ce8cd-3814-4cb0-bf1f-e994dd77f4b9)

Запуск действий на агенте 

![Desktop Screenshot 2024 12 03 - 16 43 55 32](https://github.com/user-attachments/assets/94cedf93-91a3-4cb9-9931-b6f1fc7f1884)

Логи на сервере

![Desktop Screenshot 2024 12 03 - 15 24 10 11](https://github.com/user-attachments/assets/2b3d44a2-8f7d-4d82-8c42-16d1d5771a75)

![Desktop Screenshot 2024 12 03 - 15 25 22 11](https://github.com/user-attachments/assets/4559dbe6-243a-4d0a-8923-d1c2478d2bde)


