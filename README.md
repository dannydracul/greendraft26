![](images/Pasted%20image%2020260722225245.png)
#### 1. Коммутатор C-SW
#### 1.1 show vlan brief
![](images/Pasted%20image%2020260722112724.png)
#### 1.2 show int desc
![](images/Pasted%20image%2020260722112812.png)
#### 1.3 show run | sec int
![](images/Pasted%20image%2020260722112944.png)
#### 1.4 show int trunk
![](images/Pasted%20image%2020260722131556.png)
#### 1.4 show int switchport
![](images/Pasted%20image%2020260722131745.png)
![](images/Pasted%20image%2020260722131941.png)
![](images/Pasted%20image%2020260722132008.png)
![](images/Pasted%20image%2020260722132044.png)
![](images/Pasted%20image%2020260722132129.png)
#### 1.5 show ip int br | exc unass
![](images/Pasted%20image%2020260722132229.png)
#### 1.6 show ip ssh
![](images/Pasted%20image%2020260722132318.png)
#### 1.7 show run | sec line
![](images/Pasted%20image%2020260722133041.png)
#### 1.8 show users
![](images/Pasted%20image%2020260722134149.png)
#### 1.9 show run | sec user
![](images/Pasted%20image%2020260722134246.png)
#### 1.10 show run | sec archive
![](images/Pasted%20image%2020260722134650.png)
#### 1.11 show archive
![](images/Pasted%20image%20260724072740.png)
#### 1.12 show clock
![](images/Pasted%20image%2020260722135111.png)
#### 1.13 show ntp status
![](images/Pasted%20image%2020260722135215.png)
#### 2. Маршрутизатор C-RTR
#### 2.1 show run | sec int
![](images/Pasted%20image%2020260722135843.png)
![](images/Pasted%20image%2020260722135907.png)
#### 2.2 show int desc
![](images/Pasted%20image%2020260722135950.png)
#### 2.3 show ip route
![](images/Pasted%20image%2020260722140904.png)
#### 2.4 sh ip nat translations
![](images/Pasted%20image%2020260722141112.png)
#### 2.5 show ip access-lists
![](images/Pasted%20image%2020260722141221.png)
#### 2.6 show ip ssh
![](images/Pasted%20image%2020260722141523.png)
#### 2.7 show run | sec line
![](images/Pasted%20image%2020260722143945.png)
#### 2.8 show run | sec user
![](images/Pasted%20image%2020260722144114.png)
#### 2.9 show clock
![](images/Pasted%20image%2020260722144611.png)
#### 2.10 show ntp status
![](images/Pasted%20image%2020260722145403.png)
#### 3. Сервер Linux L-SRV
#### 3.1 cat /etc/network/interfaces
![](images/Pasted%20image%2020260722155422.png)
#### 3.2 cat /etc/resolv.conf
![](images/Pasted%20image%2020260722155508.png)
#### 3.3 systemctl status tftpd-hpa (настраивал через xinetd)
![](images/Pasted%20image%2020260722160241.png)
![](images/Pasted%20image%2020260722160303.png|458)
#### 3.4 hostnamectl
![](images/Pasted%20image%2020260722160603.png)
#### 3.5 netstat -tlupn и ss -tlu
![](images/Pasted%20image%2020260722160803.png)
#### 3.6 ls -lh /opt/backups, затем делаем write memory на C-SW и снова вывод ls -lh /opt/backups
![](images/Pasted%20image%2020260722182744.png)
![](images/Pasted%20image%2020260722182952.png)
#### 3.7 cat /etc/nginx/sites-available/<содержимое конфиг файлов обоих сайтов>
![](images/Pasted%20image%2020260722161148.png)
![](images/Pasted%20image%2020260722161223.png)
#### 3.8 - curl [http://configs.greendraft26.local](http://configs.greendraft26.local/)
![](images/Pasted%20image%2020260722183133.png)
![](images/Pasted%20image%2020260722161358.png)
![](images/Pasted%20image%2020260722161425.png)
#### 3.9 cat /etc/passwd
![](images/Pasted%20image%2020260722161604.png)
#### 3.10 grep –E ‘Port|Root|Pubkey|Password’ /etc/ssh/sshd_config
![](images/Pasted%20image%2020260722161706.png)
#### 3.11 docker ps
![](images/Pasted%20image%2020260722161755.png)
#### 3.12 date
![](images/Pasted%20image%2020260722161809.png)
#### 4. Сервер Windows W-SRV
#### 4.1 ipconfig /all
![](images/Pasted%20image%2020260722183455.png)
#### 4.2 (get-timezone).id
![](images/Pasted%20image%2020260722183550.png)
#### 4.3 Get-ADDomain
![](images/Pasted%20image%2020260722183710.png)
#### 4.4 Get-DnsServerZone
![](images/Pasted%20image%2020260722183811.png)
#### 4.5 Get-DnsServerResourceRecord
![](images/Pasted%20image%2020260722184844.png)
#### 4.6 Get-DnsServerForwarder
![](images/Pasted%20image%2020260722184951.png)
#### 4.7 Get-DhcpServerv4Scope
![](images/Pasted%20image%2020260722185059.png)
#### 4.8 Get-DhcpServerv4ExclusionRange
![](images/Pasted%20image%2020260722185127.png)
#### 4.9 Get-DhcpServerv4Lease –ScopeId 10.10.10.0
![](images/Pasted%20image%2020260722190006.png)
#### 4.10 Get-ADUser DBarkov
![](images/Pasted%20image%2020260722185403.png)
#### 4.11 Get-ADComputer L-CLI -Properties OperatingSystem
![](images/Pasted%20image%2020260722185510.png)
#### 4.12 w32tm /query /source
![](images/Pasted%20image%2020260722185542.png)

#### 5. **Клиент Astra Linux L-CLI** Залогиниться под своей доменной учетной записью
#### 5.1 ip -br a
![](images/Pasted%20image%2020260722190027.png)
#### 5.2 whoami
![](images/Pasted%20image%2020260722190053.png)
#### 5.3 astra-winbind -i
![](images/Pasted%20image%2020260722191020.png)
#### 5.4 Открыть в Firefox сайт с конфигурациями [http://configs.greendraft26.local](http://configs.greendraft26.local/)
![](images/Pasted%20image%2020260722191121.png)
#### 5.5 Открыть в Firefox сайт с игрой Mario [http://mario.greendraft26.local](http://mario.greendraft26.local/)
![](images/Pasted%20image%2020260722191152.png)
#### 5.6 ssh admin@c-rtr и ssh admin@c-sw
![](images/Pasted%20image%2020260722192442.png)
![](images/Pasted%20image%2020260722193322.png)
#### 5.7 ssh –p 2026 <Ваша УЗ L-SRV>@l-srv, пример – ssh –p 2026 aivanov@l-srv
![](images/Pasted%20image%2020260722193720.png)
#### 5.8 Последовательно ping ya.ru, ping dc, ping l-srv
![](images/Pasted%20image%2020260722193817.png)
#### 5.9 nslookup vk.com и nslookup configs
![](images/Pasted%20image%2020260722193857.png)
#### 5.10 date
![](images/Pasted%20image%2020260722193915.png)
#### 6. Принтер C-PRINTER
#### 6.1 show ip, затем ip dhcp и снова show ip
![](images/Pasted%20image%2020260722194147.png)


