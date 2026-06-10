# Lesson 7 — Linux Networking Basics

## Main Concepts

IP address = адрес компьютера в сети.

127.0.0.1 = localhost.  
localhost = этот же компьютер.

DNS = перевод имени в IP.

Port = номер сервиса.

Important ports:

- 22 = SSH
- 53 = DNS
- 80 = HTTP
- 443 = HTTPS

TCP = надежный протокол.  
UDP = быстрый протокол без проверки доставки.

HTTP = без шифрования.  
HTTPS = с шифрованием.

Firewall = фильтр сетевого доступа.

0.0.0.0 = доступно извне.  
127.0.0.1 = только локально.

LISTEN = сервис ожидает подключение.

---

## Commands

```bash
ip a
ping 8.8.8.8
ping google.com
ping 127.0.0.1
ss -tuln
sudo ufw status
sudo ufw enable
sudo ufw allow 22


What I learned
IP address shows where a computer is in the network.
DNS translates domain names to IP addresses.
Ports show which services are available.
SSH uses port 22.
Open ports can be a security risk.
Firewall controls network access.
UFW is a simple firewall tool in Ubuntu.


IT English
IP address — IP адрес
localhost — локальный компьютер
DNS — domain name system
port — порт
connection — соединение
service — сервис
firewall — брандмауэр
allow — разрешить
deny — запретить
listen — ожидать подключение
SSH — secure shell
HTTP — web traffic without encryption
HTTPS — encrypted web traffic



General English

I am learning networking.
I use Linux every day.
I am using the terminal now.
There is a server.
There are open ports.
Is there a problem?
The firewall is active.
