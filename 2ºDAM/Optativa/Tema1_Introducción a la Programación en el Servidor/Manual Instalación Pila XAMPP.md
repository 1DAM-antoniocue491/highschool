## Introducción
Lo que vamos a instalar en este manual es la pila **XAMPP**.

La XAMPP tiene las siglas:
- **X:** Windows/Linux
- **A:** Apache
- **M:** Maria DB
- **P:** PHP
- **P:** PERL

Su principal utilidad es la simulación de un servidor en nuestro equipo. Con esto se pueden desplegar páginas webs completas con acceso a bases de datos locales, etc.

---
## Pasos para la instalación
1. Primero nos tenemos que ir a la página oficial de Apache Friends para obtener el ejecutable. Para ir a la página web, haga [clic aquí](https://www.apachefriends.org/es/download.html).
	![[Pasted image 20250917173458.png]]
2. Cuando tenemos el `.exe` lo ejecutamos. En la primera ventana empezaremos la configuración inicial haciendo clic en *Next*.
	![[Pasted image 20250917173744.png]]
3. En esta siguiente ventana se pueden ver todos los servicios que podemos decidir instalar o no instalar. Por defecto vienen todos los servicios señalados, por lo que hacemos clic en *Next*.
	![[Pasted image 20250917173832.png]]
4. Como podemos ver en la imagen, en esta pantalla se seleccionará la ruta absoluta donde se generará la carpeta de `xampp`. Posteriormente veremos qué contiene esta carpeta. Por defecto viene la ruta `C:\xampp`. Nosotros podemos poner la ruta que más nos interese.
	![[Pasted image 20250917174027.png]]
5. Posteriormente se indicará el idioma y al darle a *Next* se empieza a instalar la pila XAMPP.
	![[Pasted image 20250917174435.png]]
6. Finalmente ya está instalado.
	![[Pasted image 20250917174611.png]]

---
## Contenido de la carpeta `C:\xampp`
Esta es la estructura principal del directorio `C:\xampp`.
Como he comentado, es la *estructura principal*, además de estos directorios y ficheros existen otros ficheros y directorios internos.
```Shell
xampp/
├── apache/          # Archivos de configuración y módulos de Apache
├── cgi-bin/         # Scripts CGI
├── contrib/         # Archivos adicionales
├── FileZillaFTP/    # Servidor FTP (si está instalado)
├── htdocs/          # Carpeta raíz de documentos web (aquí van tus proyectos)
│   └── index.php    # Página de inicio por defecto de XAMPP
├── logs/            # Archivos de registro (errores, accesos, etc.)
├── mercury/         # Servidor de correo Mercury (opcional)
├── mysql/           # Archivos y bases de datos de MySQL/MariaDB
│   └── data/        # Aquí se almacenan las bases de datos
├── perl/            # Soporte para Perl
├── php/             # Archivos de configuración y librerías de PHP
├── phpMyAdmin/      # Aplicación web para administrar bases de datos
├── sendmail/        # Configuración para envío de correos
├── tmp/             # Archivos temporales
└── xampp-control.exe # Panel de control (solo en Windows)
```
