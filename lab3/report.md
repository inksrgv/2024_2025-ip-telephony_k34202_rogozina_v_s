University: ITMO University

Faculty: PIn

Course: IP-telephony

Year: 2024/2025

Group: K34202

Author: Rogozina Veronika Sergeevna

Lab: Lab3

Date of create: 12.03.2025

Date of finished: 14.03.2025

# Лабораторная работа №3 "Использование Asterisk в качестве SIP proxy"

## Цель работы

Изучить программный комплекс Asterisk. Настройка Asterisk для локальных звонков.

## Задание

1. Установить систему server.
   
2. Установить Asterisk.
   
3. Установить soft телефон на рабочую станцию.
   
4. Настроить SIP каналы.

5. Подключиться к SIP каналам soft телефона.

6. Сделать тестовый звонок на номер 1000
   
## Ход выполнения работы 

### Установка и настройка Asterisk

Для начала устанавливаем Asterisk

![Снимок экрана от 2025-02-19 16-23-46](https://github.com/user-attachments/assets/4aa09aa1-d032-49dd-a36d-7717a8e380c2)

После успешной установки редактируем файлы конфигурации

`sip.conf`

![Снимок экрана от 2025-03-12 14-34-37](https://github.com/user-attachments/assets/df302f7a-a656-4d3b-be03-261930a9bf04)

`extensions.conf`

![Снимок экрана от 2025-03-12 14-29-00](https://github.com/user-attachments/assets/6263d155-bf6e-4cf8-8f6d-8edc9903060b)

И перезапускаем службу

![Снимок экрана от 2025-02-19 16-31-32](https://github.com/user-attachments/assets/64bc1c99-00da-4b0d-9126-b56d8d038692)

Проверяем, что все работает

![Снимок экрана от 2025-02-19 16-32-21](https://github.com/user-attachments/assets/020e1db8-a843-4b13-b5bc-afda8b18376b)

Теперь можно переходить к следующему шагу

### Установка и настройка телефона Zoiper

Скачиваем ZoiPer5 с официального сайта и распаковываем его

![Снимок экрана от 2025-02-19 16-50-50](https://github.com/user-attachments/assets/b30dc4d8-d29e-41c0-8864-8644baa14f87)

Заходим в приложение под логином и паролем одного из созданных аккаунтов (в моем случае "111")

![Снимок экрана от 2025-02-19 17-02-27](https://github.com/user-attachments/assets/c543cfc2-e4e2-4106-a211-fced194ec441)

Проверим, что порт отображается внутри Asterisk

![Снимок экрана от 2025-02-19 17-03-36](https://github.com/user-attachments/assets/025ea53b-724e-4fa0-9dc3-49fd7936e33c)

Все хорошо, можем переходить дальше

### Установка и настройка MicroSIP

Для начала устанавливаем утилиту wine

![Снимок экрана от 2025-03-12 14-08-00](https://github.com/user-attachments/assets/e2d4ae26-5a09-4475-aa25-0a496c206745)

Затем с официального сайта скачиваем MicroSIP и с помощью утилиты wine завершаем установку

![Снимок экрана от 2025-03-12 14-14-56](https://github.com/user-attachments/assets/910bc2e2-f06f-4eeb-a5c6-c8fcfab61334)

В итоге открывается установщик, следуя инструкциям завершаем установку

![Снимок экрана от 2025-03-12 14-15-12](https://github.com/user-attachments/assets/0bd512fb-f01c-441f-9d7d-ead0c70b6cde)

После чего входим в ранее созданный аккаунт ("222")

![Снимок экрана от 2025-03-12 14-18-10](https://github.com/user-attachments/assets/452f0b70-ea44-4adc-93fa-797a411edfdc)

После чего получаем следующий вид двух телефонов:

![Снимок экрана от 2025-03-12 14-18-46](https://github.com/user-attachments/assets/62a15a80-f56f-4fd5-b06f-77f8a2193679)

Проверим, что порты отображаются корректно:

![Снимок экрана от 2025-03-12 14-20-06](https://github.com/user-attachments/assets/2c0dd0cf-b2fc-4fd7-b819-b19db4959bcf)

Проверим сетевую связность:

`111 -> 222`

![Снимок экрана от 2025-03-12 14-36-34](https://github.com/user-attachments/assets/49506eea-93d3-4b21-9acf-c85507f792c9)

`222 -> 111`

![Снимок экрана от 2025-03-12 14-36-20](https://github.com/user-attachments/assets/56214d9e-c6dc-4e41-acb3-17b019eacf1e)

## Вывод 

В ходе выполнения работы был изучен и настроен для локальных звонков программный комплекс Asterisk. 



