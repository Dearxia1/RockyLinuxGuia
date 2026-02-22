# Guía de Instalación y Configuración: Rocky Linux 9 Minimal para Servidores

| Autor | Asignatura | Institución |
| :--- | :--- | :--- |
| **Daniel Mejía** | Infraestructura III | Universidad Icesi |

¡Bienvenido a la documentación paso a paso para la instalación de **Rocky Linux 9 Minimal**!

He diseñado esta guía para que **cualquier persona**, incluso si es su primera vez usando máquinas virtuales o interactuando con Linux sin entorno gráfico (solo texto), pueda seguirla sin perderse en el intento.

A lo largo de estos capítulos, aprenderás a construir y estabilizar un servidor virtual desde cero (VirtualBox), a configurar su salida a internet de forma fija y estática por Línea de Comandos (CLI) y a gestionarlo de manera remota como lo hacen los profesionales (SSH).

## 📑 Tabla de Contenidos a Seguir:

Te recomendamos leer la guía en el siguiente orden secuencial:

1. **[Objetivos y Requisitos](./docs/01-instalacion/01-objetivos-requisitos.md)**  
   *Prepara tu entorno, los archivos ISO y conoce la meta final.*
2. **[Instalación del Sistema y Particionamiento Manual](./docs/01-instalacion/02-proceso-instalacion.md)**  
   *Cómo crear la VM, ajustar la red para que tenga internet y fraccionar los discos en Anaconda inteligentemente.*
3. **[Configuración de Red Estática por CLI (nmcli)](./docs/02-red/01-configuracion-nmcli.md)**  
   *Cómo darle a tu servidor una dirección IP fija paso a paso usando la terminal pura.*
4. **[Acceso Remoto por SSH (Cliente Host)](./docs/03-ssh/01-acceso-remoto.md)**  
   *Cómo minimizar la máquina virtual y controlarla con comandos cómodamente desde tu Windows o Mac.*
5. **[Conclusiones, Alcances y Dificultades](./docs/04-conclusiones/01-informe-final.md)**  
   *El resumen del aprendizaje, las trabas más comunes para los principiantes y las lecciones obtenidas de particiones y consola.*

---
*Este proyecto y su documentación detallada han sido desarrollados como parte de las actividades del curso de Infraestructura III en la Universidad Icesi.*
