# 📦 Bloque 2 — Detección en Red y Endpoint

[![Estado](https://img.shields.io/badge/Estado-En%20Progreso-7C6FCD?style=flat)](.)
[![Snort](https://img.shields.io/badge/Snort-IDS%20Firma-CC0000?style=flat)](.)
[![Suricata](https://img.shields.io/badge/Suricata-IDS%20Avanzado-EF3B2D?style=flat)](.)
[![YARA](https://img.shields.io/badge/YARA-Malware-8B5CF6?style=flat)](.)
[![Wazuh](https://img.shields.io/badge/Wazuh%20Agent-EDR-005571?style=flat)](.)

[← Volver al README principal](../README.md)

---

## 🎯 Objetivo del Bloque

Implementar un sistema de detección **multicapa** en VM1 que combine:

| Capa | Herramienta | Función |
|---|---|---|
| Detección por firma | Snort | Identificar patrones conocidos de ataque |
| Detección avanzada | Suricata | Análisis de protocolo y flujos |
| Detección de malware | YARA | Escaneo de archivos en disco y memoria |
| Análisis de comportamiento | Wazuh Agent | Monitorización del endpoint (EDR) |

Este bloque complementa la monitorización pasiva del Bloque 1 con **detección activa en tiempo real**.

---

## 🔴 Snort — IDS basado en firmas

### Instalación y configuración

| Campo | Valor |
|---|---|
| Versión | Snort 2.9.x |
| Red monitorizada | 192.168.20.0/24 |
| Modo | IDS pasivo |
| Config principal | `/etc/snort/snort.conf` |

```bash
# Instalación
sudo apt install snort -y

# Red monitorizada (durante instalación)
Home network: 192.168.20.0/24

# Validación de configuración
sudo snort -T -c /etc/snort/snort.conf
```

### Directorio de reglas personalizadas

```bash
sudo mkdir -p /etc/snort/rules/sentinellab
```

### Reglas personalizadas creadas

Archivo: `/etc/snort/rules/sentinellab/local.rules`

```
# ============================================
# SentinelLab — Reglas Snort personalizadas
# ============================================

# Regla 1: Detectar intentos SSH desde Kali
alert tcp any any -> 192.168.20.20 22 \
  (msg:"[SentinelLab] Intento de conexion SSH detectado"; sid:1000001; rev:1;)

# Regla 2: Detectar escaneo de puertos (SYN scan)
alert tcp any any -> 192.168.20.20 any \
  (flags:S; msg:"[SentinelLab] Posible escaneo SYN detectado"; sid:1000002; rev:1;)

# Regla 3: Detectar acceso HTTP
alert tcp any any -> 192.168.20.20 80 \
  (msg:"[SentinelLab] Acceso HTTP detectado"; sid:1000003; rev:1;)
```

### Inclusión en configuración principal

En `/etc/snort/snort.conf`, sección Step 7:

```bash
# Sustituir la línea por defecto por:
include /etc/snort/rules/sentinellab/local.rules
```

---

## 🟠 Suricata — IDS avanzado

> 🔄 *Pendiente de documentar — en progreso*

---

## 🟣 YARA — Detección de malware

> 🔄 *Pendiente de documentar — en progreso*

---

## 🔵 Wazuh Agent — Análisis de comportamiento en endpoint

> 🔄 *Pendiente de documentar — en progreso*

---

## 🧪 Pruebas realizadas y resultados

> 🔄 *Pendiente de completar — se documentarán las pruebas de Snort, Suricata, YARA y Wazuh Agent*

---

## 📌 Aprendizajes clave

> 🔄 *Se completarán al finalizar el bloque*

---

## ➡️ Siguiente bloque

[📂 Bloque 3 — Correlación en SIEM](../bloque-3-siem/README.md)
