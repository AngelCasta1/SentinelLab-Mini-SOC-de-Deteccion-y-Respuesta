# 🛡️ SentinelLab — Mini-SOC de Detección y Respuesta

![Ubuntu](https://img.shields.io/badge/Ubuntu-22.04-E95420?style=flat&logo=ubuntu&logoColor=white)
![Wazuh](https://img.shields.io/badge/Wazuh-SIEM-005571?style=flat)
![Suricata](https://img.shields.io/badge/Suricata-IDS-EF3B2D?style=flat)
![Snort](https://img.shields.io/badge/Snort-IDS-red?style=flat)
![Estado](https://img.shields.io/badge/Estado-En%20Desarrollo-yellow?style=flat)
![Bloque](https://img.shields.io/badge/Bloque-2%2F6-blue?style=flat)

Entorno casero de monitorización de seguridad construido sobre **2 máquinas virtuales**, alineado con el certificado **"Optimización y Gestión de la Monitorización de Seguridad"** de OpenWebinars.

> 🚧 **Proyecto en progreso** — este README se actualiza a medida que se completa cada bloque.

---

## 🎯 Objetivo del Proyecto

Demostrar de forma práctica un **ciclo completo de monitorización de seguridad**:

- ✅ Centralización de logs (Syslog)
- ✅ Detección activa en red y endpoint (Snort, Suricata, Wazuh)
- ⏳ Correlación en SIEM (Wazuh Server + Grafana)
- ⏳ Enriquecimiento con Threat Intelligence (AbuseIPDB, OTX, ThreatFox)
- ⏳ Gestión de vulnerabilidades (OpenVAS + DefectDojo)
- ⏳ Detection as Code (Versionado de reglas + CI/CD)

---

## 🏗️ Arquitectura del Entorno

### Diagrama de Red
<p align="center">
  <img src="IMG_Arquitectura.png" alt="Arquitectura del Mini-SOC" width="800"/>
  <br>
  <em>Diagrama de arquitectura del entorno SentinelLab</em>
</p>

## 👤 Autor

**Ángel Castaño Arias**
Técnico en Administración de Sistemas Informáticos en Red · Cisco CCNA · Ethical Hacker · Network Security
[LinkedIn](http://www.linkedin.com/in/ángel-castaño-arias-8242b8342) · [GitHub](https://github.com/AngelCasta1)
