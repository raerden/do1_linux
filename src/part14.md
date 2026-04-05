# Part 14. Работа с системными журналами

## `/var/log/dmesg`

![ncdu /home](images/part14_1.png) \ 

## `/var/log/syslog`

![ncdu /home](images/part14_2.png) \ 

## `/var/log/auth.log`

![ncdu /home](images/part14_3.png) \ 

- Jul 19 12:34:23 - время последней успешной авторизации
- пользователь john
- метод входа LOGIN через текстовую консоль (физическую, виртуальную или через SSH-сессию, работающую в режиме консоли).

### Перезапуск службы SSHd
`sudo systemctl restart ssh`

- /var/log/syslog

![ /var/log/syslog](images/part14_4.png) \ 
__**Здесь показан запись о перезапуске SSH в логе /var/log/syslog**__


- /var/log/auth.log\
авторизация sudo для перезапуска SSHd

![ /var/log/auth.log](images/part14_5.png) \ 
__**Здесь показана запись о логине sudo для перезапуска SSH в логе /var/log/auth.log**__