# Sony-Vaio-SVE14-OpenCore.
OpenCore EFI and guide for macOS Monterey on Sony Vaio SVE14113ELW
# Hackintosh Sony Vaio SVE14113ELW - Intel Core i3-2370M (Sandy Bridge)

¡Bienvenido a este repositorio! Este proyecto documenta la configuración de OpenCore para ejecutar **macOS Monterey (12.7.6)** de manera estable en una laptop clásica **Sony Vaio SVE14113ELW**[cite: 1].

---

## 💻 Especificaciones del Equipo
* **Motherboard:** SONY SVE14113ELW con chipset HM76[cite: 1]
* **Procesador (CPU):** Intel Core i3-2370M @ 2.40GHz (Arquitectura Sandy Bridge)[cite: 1]
* **Gráficos (iGPU):** Intel HD Graphics 3000 (Device ID: 8086-0116) con soporte para pantalla interna (1366x768) y salida HDMI a monitor externo[cite: 1]
* **Almacenamiento:** Disco duro Seagate ST500LM021 (500 GB) en controlador SATA[cite: 1]
* **Audio:** Realtek ALC269 (Controlador Intel High Definition Audio)[cite: 1]
* **Red / Ethernet:** Realtek PCIe GBE Family Controller[cite: 1]
* **Wi-Fi:** Qualcomm Atheros AR9485WB-EG (PCI) y adaptador USB AIC8800D80[cite: 1]
* **Bluetooth:** Qualcomm Atheros AR3012[cite: 1]
* **Controladores USB:** Intel 7 Series/C216 (Incluye puertos USB 3.0 e hilos USB 2.0)[cite: 1]
* **Otros:** Lector de tarjetas Realtek PCIE CardReader[cite: 1]

---

## 🍏 Versión de macOS
* **Sistema Operativo:** macOS Monterey 12.7.6
* **Gestor de arranque:** OpenCore

> 💡 **Nota técnica:** macOS Monterey es el límite óptimo y más avanzado para este hardware de segunda generación, logrando un rendimiento general muy bueno gracias a los parches de compatibilidad gráfica para la Intel HD 3000.

---

## 🛠️ Estado del Hardware (Qué funciona y qué no)

### ✅ Lo que funciona perfectamente:
* Aceleración gráfica completa (QE/CI) para Intel HD 3000.
* Audio integrado (Altavoces y micrófono Realtek ALC269)[cite: 1].
* Puertos USB (Controlador eXtensible USB 3.0 y Enhanced de la serie 7)[cite: 1].
* Red por cable Ethernet (Realtek)[cite: 1].
* Salida de video por HDMI (probado con monitor externo LG)[cite: 1].

### ❌ Lo que no funciona / Limitaciones:
* **Wi-Fi nativo:** La tarjeta Qualcomm Atheros interna no es compatible de forma directa con Monterey[cite: 1] 
* **Modo Suspensión (Sleep):** Inestable por limitaciones de energía del chipset HM76 con versiones modernas de macOS.

---

## 🚀 Guía de Instalación Rápida
1. Prepara tu instalador USB limpio de macOS Monterey.
2. Clona o descarga esta carpeta `EFI` y colócala en la partición EFI de tu unidad de arranque.
3. Configura tu BIOS (Legacy, Secure Boot Deshabilitado, modo SATA en AHCI)[cite: 1].

---

## ☕ Apoyo Voluntario
Este proyecto es 100% de código abierto y gratuito, creado con el fin de compartir conocimiento con la comunidad de entusiastas de los Hackintosh. 
¡Una estrella ⭐ en el repositorio también ayuda muchísimo a que más personas lo descubran!
