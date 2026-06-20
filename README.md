# SentinelLab-Mini-SOC-de-Detecci-n-y-Respuesta

Entorno casero de monitorización de seguridad construido sobre 2 máquinas virtuales, alineado con los contenidos del curso **"Optimización y Gestión de la Monitorización de Seguridad"** (OpenWebinars). 
> 🚧 Proyecto en progreso — este README se actualiza a medida que se completa cada bloque.

---

## 🎯 Objetivo

Demostrar de forma práctica un ciclo completo de monitorización de seguridad: desde la centralización de logs hasta la detección, correlación en SIEM, enriquecimiento con threat intelligence, gestión de vulnerabilidades y versionado de reglas como código.

---

## 🖥️ Arquitectura

| Máquina | Rol | SO |
|---|---|---|
| **VM 1 — Objetivo + Sensor** | Servicio SSH/web expuesto · Syslog · Snort/Suricata (IDS) · agente Wazuh | Ubuntu Server 22.04 |
| **VM 2 — SIEM y gestión** | Wazuh (SIEM) · Grafana · DefectDojo · Cortex (SOAR) | Ubuntu Server 22.04 |

El equipo atacante (Kali Linux) opera desde fuera de este entorno y no cuenta como máquina del laboratorio.

```
[ Kali - Atacante ]
        │
        ▼
[ VM1: Objetivo + Sensor ]──Syslog/Snort/Suricata/Wazuh-agent──▶[ VM2: SIEM (Wazuh + Grafana) ]
                                                                          │
                                                                          ▼
                                                          DefectDojo · Cortex · Dashboards
```

*(Diagrama ampliado pendiente — se añadirá una imagen en `/docs/arquitectura.png`)*

---

## 📋 Progreso por bloques

| Bloque | Contenido | Estado |
|---|---|---|
| 1 | Fundamentos: arquitectura y Syslog | ⬜ Pendiente |
| 2 | Detección en red/endpoint: Snort, Suricata, YARA, Wazuh | ⬜ Pendiente |
| 3 | Reglas y correlación en SIEM (Wazuh + Sigma + dashboards) | ⬜ Pendiente |
| 4 | Threat Intelligence & SOAR | ⬜ Pendiente |
| 5 | Gestión de vulnerabilidades (OpenVAS + DefectDojo) | ⬜ Pendiente |
| 6 | Detection as Code | ⬜ Pendiente |

---

## 🧱 Bloque 1 — Fundamentos y Syslog

**Qué se hizo:**
- _Pendiente de completar_

**Capturas:**
- _Pendiente_

---

## 🛡️ Bloque 2 — Detección en red y endpoint

**Qué se hizo:**
- _Pendiente de completar_

**Reglas creadas:**
- `rules/snort/` — _pendiente_
- `rules/suricata/` — _pendiente_
- `rules/yara/` — _pendiente_

**Capturas:**
- _Pendiente_

---

## 🔗 Bloque 3 — SIEM y correlación

**Qué se hizo:**
- _Pendiente de completar_

**Reglas Sigma creadas:**
- `rules/sigma/` — _pendiente_

**Métricas obtenidas:**
| Indicador | Valor |
|---|---|
| MTTD (Mean Time To Detect) | _pendiente_ |
| Falsos positivos detectados | _pendiente_ |

**Capturas del dashboard:**
- _Pendiente_

---

## 🌐 Bloque 4 — Threat Intelligence & SOAR

**Qué se hizo:**
- _Pendiente de completar_

**Fuentes OSINT utilizadas:** AbuseIPDB · OTX (AlienVault) · ThreatFox

---

## 🔍 Bloque 5 — Gestión de vulnerabilidades

**Qué se hizo:**
- _Pendiente de completar_

**Hallazgos clasificados en DefectDojo:**
- _Pendiente_

---

## ⚙️ Bloque 6 — Detection as Code

**Qué se hizo:**
- _Pendiente de completar_

---

## 📂 Estructura del repositorio

```
mini-soc-suricata-wazuh/
├── README.md
├── docs/
│   └── arquitectura.png
├── rules/
│   ├── snort/
│   ├── suricata/
│   ├── sigma/
│   └── yara/
└── scripts/
    └── (scripts de validación / CI para las reglas)
```

---

## 🧰 Herramientas utilizadas

`Syslog (rsyslog)` · `Snort` · `Suricata` · `YARA` · `Wazuh` · `Grafana` · `Sigma` · `AbuseIPDB` · `OTX` · `ThreatFox` · `Cortex` · `OpenVAS` · `DefectDojo`

---

## 🔗 Proyectos relacionados

- [TechSolutions AI — TFG ASIR](https://github.com/AngelCasta1/TechSolutions-AI) — infraestructura corporativa base sobre la que se apoya este proyecto.

---

## 👤 Autor

**Ángel Castaño Arias**
Técnico en Administración de Sistemas Informáticos en Red · Cisco CCNA · Ethical Hacker · Network Security
[LinkedIn](http://www.linkedin.com/in/ángel-castaño-arias-8242b8342) · [GitHub](https://github.com/AngelCasta1)
