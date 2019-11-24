# Реализация нейронной сети MobileNet на ПЛИС
## Запуск проекта на плате DE0-Nano
### Подключение компонентов
Для начала подключаем камеру OV7670 и LCD экран ILI9341 к плате DE0-Nano по схеме, изображенной на рисунке ниже.

![](https://github.com/korasik/SAS_LR2/blob/master/readme_img/de0-nano/de0-nano-v1.png)

Примечания:
- плата DE0-Nano должна располагаться кристаллом вверх и usb-выходом на противоположной от вас стороне;
- выход VCC_SYS на самом экране обозначен как LED;
- выходы, обозначенные 'x', не используются.

В итоге получаем примерно следующее:

![](https://github.com/korasik/SAS_LR2/blob/master/readme_img/de0-nano/1.jpg)

### Компиляция и запуск проекта
Открываем проект в Quartus Prime (путь к файлу: SAS_LR2/verilog/imp/cam_proj.qpf), выбираем версию **cam_proj**, компилируем и загружаем на плату.

***Обратите внимание, что в данном проекте есть два revisions: нам необходим cam_proj.***

Затем настраиваем камеру, наводим ее на одну из цифр, изображенных на листе бумаги, и смотрим, распознается она или нет. Пример работы показан на рисунке ниже.

![](https://github.com/korasik/SAS_LR2/blob/master/readme_img/de0-nano/2.jpg)

## Запуск проекта на плате DE1-SoC
### Подключение компонентов
Подключаем камеру OV7670 и LCD экран ILI9341 к плате DE1-SoC по схеме, изображенной на рисунке ниже.

![](https://github.com/korasik/SAS_LR2/blob/master/readme_img/de1-soc/de1-SoC.png)

Примечания:
- выход VCC_SYS на самом экране обозначен как LED;
- выходы, обозначенные 'x', не используются.

### Компиляция и запуск проекта
Открываем проект в Quartus Prime (путь к файлу: SAS_LR2/verilog/imp/cam_proj.qpf), выбираем версию **cam_proj_DE1_SoC**, компилируем и загружаем на плату.

***Обратите внимание, что в данном проекте есть два revisions: нам необходим cam_proj_DE1_SoC.***

Затем настраиваем камеру, наводим ее на одну из цифр, изображенных на листе бумаги, и смотрим, распознается она или нет. Пример работы показан на примере цифр 3, 7, 8 на рисунках ниже.

![](https://github.com/korasik/SAS_LR2/blob/master/readme_img/de1-soc/3.JPG)
![](https://github.com/korasik/SAS_LR2/blob/master/readme_img/de1-soc/7.JPG)
![](https://github.com/korasik/SAS_LR2/blob/master/readme_img/de1-soc/8.JPG)
