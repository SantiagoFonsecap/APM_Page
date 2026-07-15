<div align="center">

# Gaseo S.A.S.

### Automatización integral para una planta embotelladora en Bogotá

[![Curso](https://img.shields.io/badge/APM-2026--1S-1E293B?style=for-the-badge)](https://github.com/santiagofonsecap/APM_Page)
[![Universidad](https://img.shields.io/badge/Universidad_Nacional_de_Colombia-A8201A?style=for-the-badge)](https://unal.edu.co)
[![Sitio web](https://img.shields.io/badge/GitHub_Pages-Ver_sitio-059669?style=for-the-badge)](https://santiagofonsecap.github.io/APM_Page/)

*Del diagnóstico en planta al gemelo digital: ingeniería de automatización aplicada al sector bebidas.*

[Explorar el sitio](https://santiagofonsecap.github.io/APM_Page/) · [Ver el código](https://github.com/santiagofonsecap/APM_Page)

</div>

---

## Sobre el proyecto

**Gaseo S.A.S.** es una propuesta de ingeniería que parte de una planta embotelladora real en Bogotá. Se levantó el flujo productivo actual, se midió el desempeño y se diseña un estado futuro que integra control industrial, robótica, supervisión SCADA y un gemelo digital para validar las mejoras antes de llevarlas a planta.

---

## El reto · 🎯

| | |
|:---|:---|
| **OEE AS-IS (gaseosa / garrafón)** | 71,4% / 73,4% |
| **Operarios de fin de línea** | de 4 a 2 por turno |

Las líneas de envasado ya están automatizadas; el reto está en el **fin de línea manual** (tapado de garrafones cada 4 s y paletizado de cargas de 20–21 kg, ~36 t/h combinadas), ergonómicamente inviable. Se resuelve con dos mejoras —actuador neumático de tapado y celda robotizada de paletizado **ABB IRB 660**— y digitalización del flujo de información con SCADA en Ignition, validadas por simulación (Tecnomatix Plant Simulation) y gemelo digital.

---

## Portafolio de productos · 📦

Dos líneas de producción diferenciadas por envase, formato y velocidad de línea:

| # | Línea | Envase | Velocidad de referencia |
|---|----------|--------|------------------------|
| 1 | Gaseosa cola 400 ml (canastas × 24) | Vidrio retornable | 20 000 bot/h |
| 2 | Garrafón de agua 20 L | Retornable | 900 gar/h |

---

## Flujo del proceso (visión rápida)

```
Insumos → Clarificación → Jarabe → Mezcla → Carbonatación → Llenado → Sellado →
Etiquetado → Inspección → Empaque → Embalaje → Paletizado → Almacén → Despacho
```

---

## Los siete pilares del trabajo

Cada bloque aporta una pieza del rompecabezas: teoría, producción, planeación, robótica, digital factory, PLC y SCADA.

| Módulo | Qué cubre |
|--------|-----------|
| **1 · Introducción a la Automatización** | Marco conceptual, Industria 4.0 y niveles de automatización. |
| **2 · Gestión de Producción** | DOP, DAP, VSM, OEE, Takt Time, cuellos de botella y simulación en Tecnomatix. |
| **3 · Planeación y Evaluación** | EDT, cronograma, análisis de utilidad y viabilidad económica (CAPEX/OPEX, VPN, TIR, ROI). |
| **4 · Celdas Robotizadas** | Selección de robot (ABB IRB 660), herramienta terminal, layout de celda, balance de ciclos, RobotStudio y evaluación de riesgos (ISO 14121-1). |
| **5 · Digital Factory** | Modelado 3D en Siemens NX (MCD), sensores virtuales, mapeo de señales y arquitectura OPC. |
| **6 · Controladores industriales (PLC)** | Grafcet, lógica Ladder en Studio 5000 y validación por emulación. |
| **7 · SCADA** | ISA-101, diseño HMI en Ignition, trazabilidad de pallets y comunicación OPC. |

---

## Dónde estamos · 📍

**Ya consolidado** — Línea base del estado actual (levantamiento, diagramas, indicadores y mapa de flujo de valor), portafolio de dos líneas, evaluación económica completa (CAPEX, VPN, TIR y payback), celda robotizada ABB IRB 660 con layout, balance de ciclos y evaluación de riesgos ISO 14121-1, lógica de control (Grafcet y Ladder en Studio 5000, validada por emulación), gemelo digital en Siemens NX con mapeo de señales OPC, SCADA en Ignition (HMI y trazabilidad de pallets), pirámide ISA-95 y arquitectura de red, simulación de eventos discretos, cronograma reprogramado y sitio web multipágina.

**En construcción** — VSM del estado futuro, modelo de tags y lista de alarmas del SCADA, resultados finales de validación del gemelo digital, acciones abiertas de seguridad (cálculo del PL alcanzado y distancias de cortinas) y sustentación final (mayo 2026).

---

## Estructura del repositorio

```
APM_Page/
├── .cursor/                 # Reglas y skills para el flujo de trabajo en Cursor
├── .github/workflows/       # Despliegue continuo a GitHub Pages
├── archivos-drive/          # Material sincronizado con el drive del equipo
├── reprogramacion/          # Cronograma reprogramado
├── scripts/                 # Python (cronograma Excel) y shell (sync)
├── website/                 # Sitio estático: HTML, CSS, JS, imágenes y PDFs
├── requirements.txt
├── serve.py                 # Servidor local de desarrollo
└── APM.ods                  # Hoja de cálculo del proyecto
```

La carpeta `website/` concentra la experiencia pública: landing tipo *pitch*, propuesta técnica, evaluación económica, siete páginas de módulo, reflexiones del equipo, contacto, información de la asignatura y páginas legales.

---

## Stack y herramientas · ⚙️

**Ingeniería y planta**

| Área | Herramientas |
|------|----------------|
| Simulación | Tecnomatix Plant Simulation |
| Robótica | RobotStudio (ABB) · RAPID |
| Gemelo digital | Siemens NX — Mechatronics Concept Designer (MCD) |
| Control | Studio 5000 / RSLogix (Ladder) |
| Emulación | Logix Emulate |
| SCADA | Ignition (Inductive Automation) |
| Comunicaciones | OPC UA / OPC DA (Ignition como pasarela) · Node-RED |
| Diagramas | draw.io / diagrams.net |

**Repositorio y producto digital**

| Capa | Tecnología |
|------|------------|
| Sitio | HTML5, CSS3, JavaScript (vanilla) |
| Tipografía | Google Fonts — Outfit + Public Sans |
| Despliegue | GitHub Pages + GitHub Actions |
| Scripts | Python 3 (p. ej. openpyxl) |
| Sincronización de datos con Google Drive | rclone + bash |
| Colaboración | Cursor IDE |

**Paleta visual del proyecto**

| Rol | Hex |
|-----|-----|
| Primario (granate) | `#A8201A` |
| Primario oscuro | `#6B1410` |
| Secundario (navy) | `#1E293B` |
| Fondo | `#F8FAFC` |
| Éxito | `#059669` |
| Advertencia | `#D97706` |

---

## Ver el sitio en local · 🖥️

Desde la raíz del repositorio:

```bash
python3 serve.py
```

Por defecto el servidor escucha en el **puerto 8766**. Abre en el navegador:

**http://localhost:8766/**

Para otro puerto:

```bash
python3 serve.py 8080
```

*(Opcional)* Entorno Python para scripts:

```bash
python3 -m venv .venv && source .venv/bin/activate   # Linux/macOS
pip install -r requirements.txt
```

---

## Equipo (Grupo 4)

| # | Integrante |
|---|------------|
| 1 | Juan Esteban Otavo García |
| 2 | Santiago Camilo Fonseca Prieto |

> El proyecto continuó como un equipo de dos personas después de la primera entrega.

---

## Docentes

| Profesor | Módulo |
|----------|--------|
| Carlos Julio Cortés R. | Gestión y evaluación de la producción automatizada |
| Luis Miguel Méndez | Introducción a la Automatización / Planeación y Evaluación |
| Víctor Hugo Grisales | Automatización discreta: PLC y SCADA |
| Ricardo Ramírez H. | Celdas de manufactura robotizadas |
| Eduardo Barrera Gualdrón | Coordinación, SCADA |
| Ubaldo García Zaragoza | Digital Factory |

---

## Enlaces

| Recurso | URL |
|---------|-----|
| **Repositorio** | https://github.com/santiagofonsecap/APM_Page |
| **Sitio en vivo** | https://santiagofonsecap.github.io/APM_Page/ |

---

## Licencia

Este proyecto se distribuye bajo la [Licencia MIT](LICENSE).

Proyecto académico de la asignatura **Automatización de Procesos de Manufactura (APM)** — 2026-1S, Universidad Nacional de Colombia.

---

<div align="center">

**Gaseo S.A.S.** · *Ingeniería de bebidas, automatizada de punta a punta.*

</div>
