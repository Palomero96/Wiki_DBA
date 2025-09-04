---
title: Ubuntu
css: fullwidth
---

[MySQL](../index.md) / [Instalación](index.md) / Ubuntu
# Instalación de MySQL en Ubuntu

Bienvenido a la guía de instalación de MySQL en Ubuntu. Esta guía cubre los pasos básicos para instalar MySQL desde los repositorios oficiales.

## Índice rápido
- [Actualizar el sistema](#actualizar-el-sistema)
- [Instalar MySQL Server](#instalar-mysql-server)
- [Configurar MySQL](#configurar-mysql)
- [Iniciar y habilitar el servicio](#iniciar-y-habilitar-el-servicio)
- [Verificar la instalación](#verificar-la-instalacion)

## Actualizar el sistema
Antes de instalar cualquier paquete, actualiza la lista de paquetes:

```bash
sudo apt update && sudo apt upgrade -y
```

## Instalar MySQL Server
Instala el servidor MySQL desde los repositorios oficiales:

```bash
sudo apt install mysql-server -y
```

## Configurar MySQL
Ejecuta el script de seguridad de MySQL para configurar la contraseña del root y opciones básicas de seguridad:

```bash
sudo mysql_secure_installation
```

Sigue las instrucciones en pantalla para completar la configuración.

## Iniciar y habilitar el servicio
Asegúrate de que el servicio de MySQL esté activo y se inicie automáticamente al arrancar el sistema:

```bash
sudo systemctl start mysql
sudo systemctl enable mysql
```

## Verificar la instalación
Conéctate a MySQL para verificar que todo esté funcionando correctamente:

```bash
sudo mysql -u root -p
```

Si ves el prompt de MySQL, la instalación fue exitosa.

---




