# Пользователи и права доступа

В Linux существует три типа пользователей:
- root — это суперпользователь, у него есть права на все операции (установка, удаление программ)
- Системные пользователи — это процессы, у которых есть доступ к своим файлам и папкам
- Обычные пользователи — учетные записи пользователей, допущенных к управлению системой

Все пользователи имеют свой уникальный ID. Обычные пользователи имеют значение от 1000.

Для получения информации о пользователях системы достаточно посмотреть файл
```sh
sudo cat /etc/passwd
```

```sh
George:x:1002:1002:George Metesky:/home/george:/bin/bash
```

Для изменения, удаления, добавления пользователей необходимы права суперпользователя.

Чтобы запускать команды как суперпользователь нужно добавить ставку `sudo` перед вызовом команды.
```sh
sudo ls
```

Добавление пользователя

```sh
sudo useradd username
```
При добавлении нового пользователя создается директория /home/username
При авторизации как username, домашней директорией устанавливается /home/username

Удаление пользователя

```sh
userdel -r username
```

Для получения информации о подключенных пользователях в системе используется команда `whoami`

___


В ОС Linux при запуске терминала подгружаются переменные `env` из файла в директории /etc. Файл содержит:
- стиль для вывода строки приглашения
- [alias](http://rus-linux.net/MyLDP/consol/alias.html)
- Указание переменной [PATH](https://opensource.com/article/17/6/set-path-linux) для указания директории, в которой хранятся запускаемые приложения

___

В Linux и других Unix подобных системах каждый файл привязан к определенному пользователю или группе.
Для получения информации о владельце и правах есть команда `ls` с [флагом](https://www.opennet.ru/man.shtml?topic=ls&category=1) `-l`

```sh
ls -l
```

```text
total 16
drwxrwxr-x 3 az az 4096 Мам 18 15:43 courses
-rw-rw-r-- 1 az az 1061 Мам 11 12:45 LICENSE
-rw-rw-r-- 1 az az 1783 Мам 18 15:54 README.md
drwxrwxr-x 3 az az 4096 Мам 18 15:56 res
```

Более подробно про значение каждого столбца можно почитать [здесь](https://linuxize.com/post/how-to-list-files-in-linux-using-the-ls-command/)

Для изменения владельца используются:
```sh
chown # Для изменения пользователя владельца
chgrp # Для изменения группы
chmod # Для изменения прав доступа к запуску, чтению, изменению
```
___

### Полезные ссылки

[Развернутая статья про пользователей в Linux и про их управление](https://techlist.top/linux-users-types-of-users/)

[Команда Whoami в Linux](https://andreyex.ru/operacionnaya-sistema-linux/komanda-whoami-v-linux/)

[Изучаем команды Linux: alias](http://rus-linux.net/MyLDP/consol/alias.html)

[Оттачиваем навык использования PATH](https://opensource.com/article/17/6/set-path-linux)

[Все про ls](https://linuxize.com/post/how-to-list-files-in-linux-using-the-ls-command/)

[Права доступа к файлам и папкам](https://www.guru99.com/file-permissions.html)

[Калькулятор прав доступа](https://chmod-calculator.com/)