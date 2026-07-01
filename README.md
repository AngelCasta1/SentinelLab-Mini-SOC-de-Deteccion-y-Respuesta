<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=4B3FA0&height=160&section=header&text=SentinelLab&fontSize=48&fontColor=FFFFFF&animation=fadeIn&fontAlignY=38&desc=Mini%20SOC%20·%20Detección%20y%20Respuesta&descSize=16&descAlignY=58&descColor=C8C3F0" width="100%" />

<br/>

[![Estado](https://img.shields.io/badge/Estado-En%20Desarrollo-7C6FCD?style=for-the-badge)](.)
[![Bloque](https://img.shields.io/badge/Bloque%20Actual-2%20%2F%206-4B3FA0?style=for-the-badge)](.)
[![Plataforma](https://img.shields.io/badge/OpenWebinars-Certificado-5E4DB2?style=for-the-badge)](.)

<br/>

[![Ubuntu](https://img.shields.io/badge/Ubuntu-22.04-E95420?style=flat&logo=ubuntu&logoColor=white)](.)
[![Wazuh](https://img.shields.io/badge/Wazuh-SIEM-005571?style=flat&logo=wazuh&logoColor=white)](.)
[![Suricata](https://img.shields.io/badge/Suricata-IDS-EF3B2D?style=flat)](.)
[![Snort](https://img.shields.io/badge/Snort-IDS-CC0000?style=flat)](.)
[![Grafana](https://img.shields.io/badge/Grafana-Dashboards-F46800?style=flat&logo=grafana&logoColor=white)](.)
[![Sigma](https://img.shields.io/badge/Sigma-Rules-4B3FA0?style=flat)](.)
[![YARA](https://img.shields.io/badge/YARA-Malware-8B5CF6?style=flat)](.)
[![Kali](https://img.shields.io/badge/Kali-Atacante-268BEE?style=flat&logo=kalilinux&logoColor=white)](.)

</div>

---

## 🎯 Objetivo

Entorno casero de monitorización de seguridad que recorre de forma práctica los **6 bloques** del certificado **"Optimización y Gestión de la Monitorización de Seguridad"** de OpenWebinars. Construido sobre 2 VMs y documentado con informe técnico completo.

📎 **[Descargar Informe Técnico PDF](__SentinelLab-MiniSOC-Informe-Técnico.pdf)**

---

## 🏗️ Arquitectura

<div align="center">
  <img src="IMG_Arquitectura.png" alt="Arquitectura SentinelLab" width="820"/>
  <br/>
  <sub>Red interna · 192.168.20.0/24 · VM1 (Objetivo + Sensores) · VM2 (SIEM + Gestión) · Kali (Atacante)</sub>
</div>

<br/>

---

## 📋 Progreso

| # | Bloque | Documentación | Estado |
|---|---|---|---|
| 1 | Fundamentos y Syslog | [📂 bloque-1-syslog](./bloque-1-syslog/) | ✅ Completado |
| 2 | Detección en red y endpoint | [📂 bloque-2-deteccion](./bloque-2-deteccion/) | 🔄 En progreso |
| 3 | Correlación en SIEM | [📂 bloque-3-siem](./bloque-3-siem/) | ⏳ Pendiente |
| 4 | Threat Intelligence & SOAR | [📂 bloque-4-threat-intel](./bloque-4-threat-intel/) | ⏳ Pendiente |
| 5 | Gestión de vulnerabilidades | [📂 bloque-5-vulnerabilidades](./bloque-5-vulnerabilidades/) | ⏳ Pendiente |
| 6 | Detection as Code | [📂 bloque-6-dac](./bloque-6-dac/) | ⏳ Pendiente |

> Cada carpeta contiene su propio README con configuraciones, capturas y resultados detallados.

---

## 🛠️ Stack tecnológico

| Categoría | Herramienta |
|---|---|
| Logs | rsyslog |
| IDS Red | Snort · Suricata |
| IDS Endpoint | Wazuh Agent |
| Detección Malware | YARA |
| SIEM | Wazuh Server |
| Visualización | Grafana |
| Reglas correlación | Sigma |
| Threat Intel | AbuseIPDB · OTX · ThreatFox |
| SOAR | Cortex |
| Vulnerabilidades | OpenVAS · DefectDojo |

---

## 🔗 Proyectos relacionados

[**TechSolutions AI — TFG ASIR**](https://github.com/AngelCasta1/TechSolutions-AI) — Infraestructura corporativa virtualizada sobre la que se apoya este proyecto.

---

<div align="center">

**Ángel Castaño Arias**

Técnico ASIR · Cisco CCNA 1·2·3 · Ethical Hacker · Network Security

[![LinkedIn](https://img.shields.io/badge/LinkedIn-4B3FA0?style=for-the-badge&logo=linkedin&logoColor=white)](http://www.linkedin.com/in/ángel-castaño-arias-8242b8342)
[![GitHub](https://img.shields.io/badge/GitHub-0d1117?style=for-the-badge&logo=github&logoColor=white)](https://github.com/AngelCasta1)

<img src="https://capsule-render.vercel.app/api?type=waving&color=4B3FA0&height=100&section=footer" width="100%" />

</div>
