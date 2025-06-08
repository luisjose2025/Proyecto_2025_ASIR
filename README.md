
# Proyecto LuJoNet

Simulación de la infraestructura de red del Departamento de Informática del IES Fernando Aguilar Quignon.

## 🧠 Descripción del Proyecto

Este Trabajo de Fin de Ciclo tiene como objetivo replicar y analizar la infraestructura de red del IES Fernando Aguilar Quignon utilizando herramientas de virtualización (Kathara). La red se segmenta mediante VLANs y proporciona servicios esenciales como DHCP, DNS, LDAP, SSSD, FTP y Autofs, con el fin de evaluar su rendimiento, seguridad y escalabilidad.

## 🛠️ Estructura del Repositorio

```
├── DHCP/lujonet/etc/dhcp         # Configuración del servidor DHCP
├── DNS                           # Configuración del servidor DNS (BIND9)
├── Dispositivos_dentro_de_la_Red # Inventario y análisis de dispositivos
├── Docker                        # Scripts y archivos para virtualización con Docker
├── Interfaces                    # Configuración de interfaces de red
├── PROYECTO                      # Documentación general del proyecto
├── bind                          # Archivos de zonas y configuración de DNS
├── install.sh                    # Script de instalación de dependencias
├── script.ldif                   # Configuración del árbol LDAP
├── sssd.conf                     # Configuración de autenticación SSSD
├── README.md                     # Este archivo
└── Instrucciones.md              # Guía detallada de instalación y uso
```

## ⚙️ Servicios Configurados

- **DHCP:** Asignación dinámica de IP por subred/VLAN.
- **DNS:** Resolución de nombres (directa e inversa) mediante BIND9.
- **LDAP + SSSD:** Autenticación centralizada de usuarios.
- **FTP:** Servicio de transferencia de archivos.
- **Autofs:** Montaje automático de directorios remotos.
- **VLANs y Routing:** Separación lógica de la red y enrutamiento entre VLANs.

## 🧪 Tecnologías y Herramientas

- Ubuntu Server (VirtualBox/Kathara)
- BIND9
- ISC DHCP Server
- OpenLDAP
- SSSD
- VSFTPD
- AutoFS
- Netplan

## 🗂️ Alcance del Proyecto

- 🔌 Segmentación de red mediante VLANs
- 📡 Configuración de múltiples subredes
- 🔐 Servicios de autenticación y seguridad básica
- 📊 Pruebas de rendimiento y conectividad
- ❌ No se incluye: IPv6, servicios web o redes Wi-Fi reales

## 📋 Requisitos

- VirtualBox o entorno compatible con Kathara
- Sistemas Linux (preferentemente Ubuntu)
- Acceso a la terminal con privilegios administrativos

## 🚀 Instalación Rápida

```bash
chmod +x install.sh
./install.sh
```

Consulta `Instrucciones.md` para una guía paso a paso.

## 👨‍💻 Autores

- **Luis Manuel Vadillo Vargas**
- **José Manuel Lizana Montero**

Trabajo realizado para el ciclo formativo de grado superior de Administración de Sistemas Informáticos en Red (ASIR).

---
