# 📝 Brutus

### HackTheBox — Sherlocks

**Nivel:** Muy fácil  
**Fecha:** 2025-10-30

---

## 🔎 Descripción (EN)
In this very easy Sherlock, you will familiarize yourself with Unix `auth.log` and `wtmp` logs. We'll explore a scenario where a Confluence server was brute-forced via its SSH service. After gaining access to the server, the attacker performed additional activities, which we can track using `auth.log`. Although `auth.log` is primarily used for brute-force analysis, we will delve into the full potential of this artifact in our investigation, including aspects of privilege escalation, persistence, and even some visibility into command execution.

---

## 🔎 Descripción (ES)
En este sencillo ejercicio de Sherlock, te familiarizarás con los registros `auth.log` y `wtmp` de Unix. Exploraremos un escenario en el que un servidor Confluence fue atacado mediante fuerza bruta a través de su servicio SSH. Tras obtener acceso al servidor, el atacante realizó actividades adicionales, que podremos rastrear utilizando `auth.log`. Aunque `auth.log` se utiliza principalmente para el análisis de fuerza bruta, profundizaremos en todo el potencial de este artefacto en nuestra investigación, incluyendo escalada de privilegios, persistencia e incluso cierta visibilidad sobre ejecución de comandos.

---
<!-- y
## 📁 Artefactos relevantes
- `/var/log/auth.log` — Autenticación SSH, sudo, su, etc.  
- `/var/log/wtmp` — Registra logins/logouts (uso con `last`).  
- `~/.ssh/authorized_keys` — Posible persistencia vía clave SSH.  
- Otros logs (opcionales): `/var/log/syslog`, `~/.bash_history`.

 -->
