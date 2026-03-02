
# 🔎 Port Scanner + Banner Grabber

### Tarea de Hacking Ético

Herramienta desarrollada como práctica de ciberseguridad para combinar **escaneo de puertos** y **captura de banners**, permitiendo identificar servicios activos y posibles versiones vulnerables en un sistema objetivo.

---

## 📌 Descripción del Proyecto

Este proyecto implementa una herramienta en Python que:

* 🔍 Escanea puertos del **1 al 200**
* 📡 Detecta cuáles están abiertos
* 🏷 Captura banners de los servicios activos

---

### 1️⃣ Port Scanner

* Escanea los puertos del **1 al 200**
* Intenta establecer conexión TCP con cada puerto
* Detecta qué puertos están abiertos

---

### 2️⃣ Banner Grabber

* Si el puerto está abierto:

  * Envía una solicitud básica al servicio
  * Captura el banner de respuesta

---

### 3️⃣ Herramienta Combinada

Integra ambas funcionalidades para:

* Detectar servicios en ejecución
* Identificar versiones expuestas
* Analizar posibles riesgos de seguridad

---

## ⚙️ Proceso de Escaneo

El script funciona de la siguiente manera:

1. Itera sobre cada puerto del 1 al 200.
2. Intenta conectarse usando **sockets TCP**.
3. Si la conexión es exitosa:

   * Marca el puerto como abierto.
   * Intenta obtener el banner del servicio.
4. Implementa un **timeout de 2 segundos** para:

   * Evitar bloqueos
   * Manejar puertos sin respuesta

---


## 🎯 Objetivos de Aprendizaje

* Comprender el funcionamiento interno de un escáner de puertos
* Entender cómo los servicios exponen información mediante banners
* Aplicar conceptos básicos de:

  * Redes
  * TCP/IP
  * Seguridad ofensiva
