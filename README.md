### КОНФИГ для ПРОШИВКИ LKIPPER для 3Д Принтера FlyingBear Ghost 6
Конфигурация открытой популярной продвинутой прошивки <a href="https://github.com/Klipper3d/klipper">Klipper</a> для 3д принтера FlyingBear Ghost 6.
Конфиг подготовлен для ревизии принтера июнь 2022г. с платой управления MKS Nano4 V3.1
Конфиг создан дополнительно к данному <a href="https://youtu.be/SGCftedVqmc">ВИДЕО</a> на ютуб канале "Уголок Технаря", многие ответы на вопросы найдете в нем.

### ИСПОЛЬЗОВАНИЕ ПРОШИВКИ
* Данные кодописания можно использовать и для прочих 3д принтеров для реализации всякого полезного функционала.
* Конфигурация разбита по файлам, если это вам не нравится, можете соединить во едино, это ваш выбор

### ЗАВИСИМОСТЬ ОТ ИСПОЛЬЗУЕМОГО ХОСТА
Абсолютно ни каким образом конфигурация не привязана к выбранному железу, кроме строк -
serial: /dev/ttyS3 в разделе [mcu] в файле printer.cfg
и строк 
* [temperature_sensor orange_pi]
* sensor_type: temperature_host
* min_temp: 10
* max_temp: 100

* [temperature_sensor mcu_temp]
* sensor_type: temperature_mcu
* min_temp: 0
* max_temp: 100

Если прошивка будет ругаться на них, просто удалите или закомментируйте их.

### КАК НАСТРОИТЬ КОНФИГ КОМПИЛЯЦИИ ПРОШИВКИ ДЛЯ ПЛАТЫ УПРАВЛЕНИЯ
![Настройка конфига компиляции](https://github.com/Technarrus/Klipper_FBG6/blob/main/menu_config.jpg)

### РЕСУРСЫ И СТАТЬИ КОТОРЫЕ ВАМ ПОМОГУТ
* Много полезного по FlyingBear Ghost6 в репозиториях товарища Том Томича: https://github.com/Tombraider2006
* Общие пояснения о прошивке и установке на хосты: https://klipper.wiki/
* Установка прошивки Klipper и прочие инструкции по настройкам полезного на сайте Кирилла OxyGena: https://fdmprint.ru/category/poleznoe/klipper/
* Подключение стокового экрана MKS к хосту и вывод на него KlipperScreen: https://sergey1560.github.io/fb4s_howto/mks_ts35/

### Связь
Вопросы, обсуждения, предложения через следующие сообщества:
* [Telegram группа](https://t.me/technarr)
* [Группа в VK](https://vk.com/technarrus)
