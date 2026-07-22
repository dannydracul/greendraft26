![](images/images/Pasted image 20260722225245.png)
#### 1. Коммутатор C-SW
###### 1.1 show vlan brief
![](images/images/Pasted image 20260722112724.png)
###### 1.2 show int desc
![](images/images/Pasted image 20260722112812.png)
###### 1.3 show run | sec int
![](images/images/Pasted image 20260722112944.png)
###### 1.4 show int trunk
![](images/images/Pasted image 20260722131556.png)
###### 1.4 show int switchport
![](images/images/Pasted image 20260722131745.png)
![](images/images/Pasted image 20260722131941.png)
![](images/images/Pasted image 20260722132008.png)
![](images/images/Pasted image 20260722132044.png)
![](images/images/Pasted image 20260722132129.png)
###### 1.5 show ip int br | exc unass
![](images/images/Pasted image 20260722132229.png)
###### 1.6 show ip ssh
![](images/images/Pasted image 20260722132318.png)
###### 1.7 show run | sec line
![](images/images/Pasted image 20260722133041.png)
###### 1.8 show users
![](images/images/Pasted image 20260722134149.png)
###### 1.9 show run | sec user
![](images/images/Pasted image 20260722134246.png)
###### 1.10 show run | sec archive
![](images/images/Pasted image 20260722134650.png)
###### 1.11 show archive
###### ![](images/images/Pasted image 20260722134418.png|989) 
###### 1.12 show clock
![](images/images/Pasted image 20260722135111.png)
###### 1.13 show ntp status
![](images/images/Pasted image 20260722135215.png)
#### 2. Маршрутизатор C-RTR
###### 2.1 show run | sec int
![](images/images/Pasted image 20260722135843.png)
![](images/images/Pasted image 20260722135907.png)
###### 2.2 show int desc
![](images/images/Pasted image 20260722135950.png)
###### 2.3 show ip route
![](images/images/Pasted image 20260722140904.png)
###### 2.4 sh ip nat translations
![](images/images/Pasted image 20260722141112.png)
###### 2.5 show ip access-lists
![](images/images/Pasted image 20260722141221.png)
###### 2.6 show ip ssh
![](images/images/Pasted image 20260722141523.png)
###### 2.7 show run | sec line
![](images/images/Pasted image 20260722143945.png)
###### 2.8 show run | sec user
![](images/images/Pasted image 20260722144114.png)
###### 2.9 show clock
![](images/images/Pasted image 20260722144611.png)
###### 2.10 show ntp status
![](images/images/Pasted image 20260722145403.png)
#### 3. Сервер Linux L-SRV
###### 3.1 cat /etc/network/interfaces
![](images/images/Pasted image 20260722155422.png)
###### 3.2 cat /etc/resolv.conf
![](images/images/Pasted image 20260722155508.png)
###### 3.3 systemctl status tftpd-hpa (настраивал через xinetd)
![](images/images/Pasted image 20260722160241.png)
![](images/images/Pasted image 20260722160303.png|458)
###### 3.4 hostnamectl
![](images/images/Pasted image 20260722160603.png)
###### 3.5 netstat -tlupn и ss -tlu
![](images/images/Pasted image 20260722160803.png)
###### 3.6 ls -lh /opt/backups, затем делаем write memory на C-SW и снова вывод ls -lh /opt/backups
![](images/images/Pasted image 20260722182744.png)
![](images/images/Pasted image 20260722182952.png)
###### 3.7 cat /etc/nginx/sites-available/<содержимое конфиг файлов обоих сайтов>
![](images/images/Pasted image 20260722161148.png)
![](images/images/Pasted image 20260722161223.png)
###### 3.8 - curl [http://configs.greendraft26.local](http://configs.greendraft26.local/)
![](images/images/Pasted image 20260722183133.png)
![](images/images/Pasted image 20260722161358.png)
![](images/images/Pasted image 20260722161425.png)
###### 3.9 cat /etc/passwd
![](images/images/Pasted image 20260722161604.png)
###### 3.10 grep –E ‘Port|Root|Pubkey|Password’ /etc/ssh/sshd_config
![](images/images/Pasted image 20260722161706.png)
###### 3.11 docker ps
![](images/images/Pasted image 20260722161755.png)
###### 3.12 date
![](images/images/Pasted image 20260722161809.png)
#### 4. Сервер Windows W-SRV
###### 4.1 ipconfig /all
![](images/images/Pasted image 20260722183455.png)
###### 4.2 (get-timezone).id
![](images/images/Pasted image 20260722183550.png)
###### 4.3 Get-ADDomain
![](images/images/Pasted image 20260722183710.png)
###### 4.4 Get-DnsServerZone
![](images/images/Pasted image 20260722183811.png)
###### 4.5 Get-DnsServerResourceRecord
![](images/images/Pasted image 20260722184844.png)
###### 4.6 Get-DnsServerForwarder
![](images/images/Pasted image 20260722184951.png)
###### 4.7 Get-DhcpServerv4Scope
![](images/images/Pasted image 20260722185059.png)
###### 4.8 Get-DhcpServerv4ExclusionRange
![](images/images/Pasted image 20260722185127.png)
###### 4.9 Get-DhcpServerv4Lease –ScopeId 10.10.10.0
![](images/images/Pasted image 20260722190006.png)
###### 4.10 Get-ADUser DBarkov
![](images/images/Pasted image 20260722185403.png)
###### 4.11 Get-ADComputer L-CLI -Properties OperatingSystem
![](images/images/Pasted image 20260722185510.png)
###### 4.12 w32tm /query /source
![](images/images/Pasted image 20260722185542.png)

#### 5. **Клиент Astra Linux L-CLI** Залогиниться под своей доменной учетной записью
###### 5.1 ip -br a
![](images/images/Pasted image 20260722190027.png)
###### 5.2 whoami
![](images/images/Pasted image 20260722190053.png)
###### 5.3 astra-winbind -i
![](images/images/Pasted image 20260722191020.png)
###### 5.4 Открыть в Firefox сайт с конфигурациями [http://configs.greendraft26.local](http://configs.greendraft26.local/)
![](images/images/Pasted image 20260722191121.png)
###### 5.5 Открыть в Firefox сайт с игрой Mario [http://mario.greendraft26.local](http://mario.greendraft26.local/)
![](images/images/Pasted image 20260722191152.png)
###### 5.6 ssh admin@c-rtr и ssh admin@c-sw
![](images/images/Pasted image 20260722192442.png)
![](images/images/Pasted image 20260722193322.png)
###### 5.7 ssh –p 2026 <Ваша УЗ L-SRV>@l-srv, пример – ssh –p 2026 aivanov@l-srv
![](images/images/Pasted image 20260722193720.png)
###### 5.8 Последовательно ping ya.ru, ping dc, ping l-srv
![](images/images/Pasted image 20260722193817.png)
###### 5.9 nslookup vk.com и nslookup configs
![](images/images/Pasted image 20260722193857.png)
###### 5.10 date
![](images/images/Pasted image 20260722193915.png)
#### 6. Принтер C-PRINTER
###### 6.1 show ip, затем ip dhcp и снова show ip
![](images/images/Pasted image 20260722194147.png)


