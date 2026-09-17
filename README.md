# 📻 LDG AT-600ProII Control para Windows

[![Plataforma](https://img.shields.io/badge/Platform-Windows%2010%20%7C%2011-blue.svg)](https://microsoft.com)
[![Lenguaje](https://img.shields.io/badge/Python-3.x-green.svg)](https://python.org)
[![Licencia](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

**Control LDG AT-600ProII** es una aplicación de escritorio desarrollada para la gestión, control y monitoreo en tiempo real del sintonizador automático de antenas **LDG AT-600ProII** mediante interfaz serie RS-232.

Diseñado pensando en la usabilidad y la fiabilidad en el cuarto de radio (*Shack*), el programa simula de manera precisa las funciones del panel frontal del equipo e integra telemetría analógica de alta precisión para el análisis de potencia de Radiofrecuencia (RF).

---

## 🚀 Características Principales

### ⚙️ Control Total del Hardware
* **Selección de Antenas (1 / 2):** Conmutación explícita mediante un algoritmo de sincronización síncrona que valida la posición física de los relés internos del equipo, evitando desalineaciones con la interfaz visual.
* **Sintonización Avanzada:** Ejecución de sintonización rápida desde memoria (*Memory Tune*) y sintonización completa (*Full Tune*).
* **Modo Bypass:** Alternancia instantánea entre modo acoplado y paso directo (*Passthru*).

### 📊 Telemetría y Medición en Tiempo Real
* **Potencia Directa (FWD):** Cálculo ajustado de potencia en vatios con corrección de compresión no lineal para lecturas de alta potencia (hasta 600 W).
* **Potencia Reflejada (REF):** Indicación continua de la potencia retornada al transmisor.
* **Lectura de ROE (VSWR):** Cálculo dinámico de la Relación de Onda Estacionaria con codificación de colores de seguridad:
  * 🟢 **Verde:** ROE < 1.5
  * 🟠 **Naranja:** ROE < 2.0
  * 🔴 **Rojo:** ROE > 2.0
* **Identificación de Banda:** Detección de la frecuencia de RF entrante en tiempo real (de 160 m a 6 m).

### 🖥️ Interfaz de Usuario y Ajustes
* **Soporte Multilingüe:** Cambio dinámico e instantáneo entre **Español** e **Inglés**.
* **Gestión de Puertos COM:** Selección y actualización de puertos serie en tiempo real desde el menú superior de configuración.
* **Persistencia de Estado:** Memorización automática en `config.json` del último puerto COM conectado, la antena activa y el idioma seleccionado.
* **Autoconexión Inteligente:** Reconexión automática con el equipo al iniciar la aplicación.

---

## 💻 Requisitos del Sistema

* **Sistema Operativo:** Windows 10 / 11 (32 o 64 bits).
* **Conexión Hardware:** Puerto RS-232 (o adaptador USB a Serie) configurado con los siguientes parámetros:
  * **Baudios:** `38400`
  * **Bits de Datos:** `8`
  * **Paridad:** `Ninguna (N)`
  * **Bits de Parada:** `1` (`38400 8N1`)

---

## 🛠️ Instalación

1. Descarga la última versión del instalador desde la sección de [Releases](../../releases).
2. Ejecuta `Instalador_LDG_Control_v1.0.exe` y sigue las instrucciones en pantalla.
3. Conecta tu cable serie a la PC y al sintonizador LDG AT-600ProII.
4. Abre la aplicación, selecciona el puerto COM correspondiente desde la barra de menú **Configuración > Puerto COM** ¡y listo!

---

👨‍💻 **Desarrollado por [CE3MRO](https://github.com/ce3mro)**
