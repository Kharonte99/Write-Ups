# 📝 Brutus

### HackTheBox — Sherlocks

**Nivel:** Muy fácil  
**Fecha:** 2025-10-30


## 🔎 Descripción (EN)
In this very easy Sherlock, you will familiarize yourself with Unix `auth.log` and `wtmp` logs. We'll explore a scenario where a Confluence server was brute-forced via its SSH service. After gaining access to the server, the attacker performed additional activities, which we can track using `auth.log`. Although `auth.log` is primarily used for brute-force analysis, we will delve into the full potential of this artifact in our investigation, including aspects of privilege escalation, persistence, and even some visibility into command execution.


## 🔎 Descripción (ES)
En este sencillo ejercicio de Sherlock, te familiarizarás con los registros `auth.log` y `wtmp` de Unix. Exploraremos un escenario en el que un servidor Confluence fue atacado mediante fuerza bruta a través de su servicio SSH. Tras obtener acceso al servidor, el atacante realizó actividades adicionales, que podremos rastrear utilizando `auth.log`. Aunque `auth.log` se utiliza principalmente para el análisis de fuerza bruta, profundizaremos en todo el potencial de este artefacto en nuestra investigación, incluyendo escalada de privilegios, persistencia e incluso cierta visibilidad sobre ejecución de comandos.


Antes de empezar repasaremos lo imprescindible de los campos del auth.log

Un "auth log" (registro de autenticación) es un archivo que registra todos los eventos relacionados con la autenticación y autorización de un sistema, como inicios de sesión, intentos de acceso, uso de comandos sudo, etc. 
En sistemas operativos Linux, se encuentra comúnmente en /var/log/auth.log


Task 1) Analyze the auth.log. What is the IP address used by the attacker to carry out a brute force attack?

Task 2) The bruteforce attempts were successful and attacker gained access to an account on the server. What is the username of the account?

Task 3) Identify the UTC timestamp when the attacker logged in manually to the server and established a terminal session to carry out their objectives. The login time will be different than the authentication time, and can be found in the wtmp artifact.

Task 4) SSH login sessions are tracked and assigned a session number upon login. What is the session number assigned to the attacker's session for the user account from Question 2?

Task 5) The attacker added a new user as part of their persistence strategy on the server and gave this new user account higher privileges. What is the name of this account?

Task 6) What is the MITRE ATT&CK sub-technique ID used for persistence by creating a new account?

Task 7) What time did the attacker's first SSH session end according to auth.log?

Task 8) The attacker logged into their backdoor account and utilized their higher privileges to download a script. What is the full command executed using sudo?




<!-- y
## 📁 Artefactos relevantes
- `/var/log/auth.log` — Autenticación SSH, sudo, su, etc.  
- `/var/log/wtmp` — Registra logins/logouts (uso con `last`).  
- `~/.ssh/authorized_keys` — Posible persistencia vía clave SSH.  
- Otros logs (opcionales): `/var/log/syslog`, `~/.bash_history`.

 -->
