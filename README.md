# Script-nmap-scan-ms17-010
# مرحبا هادا السكربث نقدر نعتبرة جميل  يفحص تغرة MS17-010
# ولكن  بحكم nmap
# مابتبين بالتفصيل 
# المهم تابع بصور لوضع الملف وكيف الفحص بيه 
![screenshot from 2017-05-22 13-46-56](https://cloud.githubusercontent.com/assets/25440152/26317402/a44aeadc-3f17-11e7-862a-01c923d9c653.png)

![screenshot from 2017-05-22 13-47-04](https://cloud.githubusercontent.com/assets/25440152/26317403/a4ddb8b2-3f17-11e7-9ed2-b8c3c44c749e.png)

![screenshot from 2017-05-22 13-47-13](https://cloud.githubusercontent.com/assets/25440152/26317405/a6192d06-3f17-11e7-81fa-62cbd06629b9.png)

![screenshot from 2017-05-22 13-47-21](https://cloud.githubusercontent.com/assets/25440152/26317407/a756c750-3f17-11e7-9c50-fc85dcd5c1d3.png)

![screenshot from 2017-05-22 13-47-27](https://cloud.githubusercontent.com/assets/25440152/26317410/a8369df8-3f17-11e7-814d-893ee0d1049d.png)

![screenshot from 2017-05-22 13-47-36](https://cloud.githubusercontent.com/assets/25440152/26318120/4bd4f4d0-3f1a-11e7-9f12-9b6c0e8a4400.png)

![Uploading Screenshot from 2017-05-22 13-47-50.png…]()
# اد  يوجد تغرة MS17-010 
# على جهاز الهدف هيطلعلك  
# nmap -Pn -sC -p445 --open --max-hostgroup 3 --script smb-vuln-ms17-010.nse 192.168.15.130

Starting Nmap 7.40 ( https://nmap.org ) at 2017-05-22 22:025 EDT
Nmap scan report for 192.168.15.130
Host is up (0.00069s latency).
PORT    STATE SERVICE
445/tcp open  microsoft-ds

Host script results:
| smb-vuln-ms17-010: 
|   VULNERABLE:
|   Remote Code Execution vulnerability in Microsoft SMBv1 servers (ms17-010)
|     State: VULNERABLE
|     IDs:  CVE:CVE-2017-0143
|     Risk factor: HIGH
|       A critical remote code execution vulnerability exists in Microsoft SMBv1
|        servers (ms17-010).
|       
|     Disclosure date: 2017-03-14
|     References:
|       https://technet.microsoft.com/en-us/library/security/ms17-010.aspx
|       https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2017-0143
|_      https://blogs.technet.microsoft.com/msrc/2017/05/12/customer-guidance-for-wannacrypt-attacks/

Nmap done: 1 IP address (1 host up) scanned in 0.59 seconds
# واد مغلقة التغرة هيطلعلك 
nmap -Pn -sC -p445 --open --max-hostgroup 3 --script smb-vuln-ms17-010.nse 192.168.15.130

Starting Nmap 7.12 ( https://nmap.org ) at 2017-22:025 CEST
Nmap scan report for 192.168.15.130
Host is up (0.00049s latency).
PORT    STATE SERVICE
445/tcp open  microsoft-ds
MAC Address: 50:7B:9D:D5:05:CA (Lcfc(hefei) Electronics Technology)
Host script results:
|_smb-vuln-ms17-010: Could not connect to 'IPC$'
















