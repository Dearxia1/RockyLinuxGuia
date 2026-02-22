# Conclusiones, Alcances y Dificultades del Proyecto

Este documento resume los resultados obtenidos tras la instalación y configuración completa del entorno de nivel servidor sobre Rocky Linux 9, abordando de manera reflexiva todo el nuevo aprendizaje, así como las barreras técnicas encontradas a lo largo de la práctica.

## 🎯 ¿Qué Logramos? (Alcances)

1. **Despliegue Exitoso sin Interfaz Gráfica:** Se logró instalar y estabilizar exitosamente una máquina virtual desde cero priorizando recursos (Instalación Mínima).
2. **Control Total del Almacenamiento:** Abandonamos la instalación "siguiente-siguiente", aprendiendo a crear y formatear discos fraccionados desde cero. Esto nos permitió asignar el particionamiento exacto (Independizando lo esencial de `/boot` y resguardándonos con el `Swap` de seguridad), demostrando madurez técnica.
3. **Gestión Remota Estabilizada:** Transitamos con éxito desde la visión limitante de VirtualBox a una consola "real" externa conectada en tiempo real. Al usar SSH y la línea de comandos para dotar de una IP inamovible (estática) al servidor, logramos mimetizar un ambiente verdaderamente profesional y listo para alojar servicios a nivel empresa.

## 🚧 Dificultades o Retos Encontrados

- **Aislamiento de VirtualBox a la Red Real:** Entender la diferencia entre darle salida a Internet a la máquina virtual (vía NAT) versus lograr que mi computador la detectara como "otra máquina independiente en mi cuarto" (Adaptador Puente) exigió revisar a fondo la configuración de red virtual del hipervisor.
- **Sintaxis Exigente en la Consola:** Comprender que las órdenes de `nmcli` deben tener espacios, mayúsculas y puntos precisos. Entender que alterar el DNS o la Puerta de Enlace sin previo aviso de cómo subir o bajar la placa lógica (reiniciarla con `CONNECTION UP`) conllevaba a la pérdida momentánea del internet dentro de la VM.
- **Acostumbramiento al Teclado Ciego de Seguridad (SSH/Root):** Generó ruido y extrañeza la dinámica nativa de Linux de no graficar con "asteriscos" ni con caracteres visiblemente interactivos el tecleo de las contraseñas para los administradores.

## 💡 Conclusión y Aprendizajes Finales

1. Entender el particionamiento interno de Linux proporciona una ventaja tremenda al momento de recuperar datos. Separar el directorio que hace que el kernel/PC encienda (`/boot`), del directorio donde están nuestros archivos comunes y toda la jerarquía de las carpetas (`/`), nos garantiza que una caída grave de un servicio instalado raramente va a matar nuestra capacidad para encender la máquina físicamente y repararla.
2. El uso temprano de las herramientas por Línea de Comandos (`NetManager` e `ip a`) optimizó el flujo de trabajo en la segunda meta del marco de red. Acostumbrarse a la CLI forja el carácter de aquellos orientados a ser ingenieros de sistemas o SysAdmins, pues es en interfaces text-only (headless) donde la eficiencia destaca sobre las nubes que consumen recursos visuales.


---
### 🤝 ¡Gracias por seguir esta guía de principio a fin!
[⬅️ Anterior: Acceso Remoto por SSH](../03-ssh/01-acceso-remoto.md) | [🏠 Volver al Inicio (README)](../../README.md)
