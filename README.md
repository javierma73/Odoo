# Odoo
¿Qué es y para qué sirve Odoo?
Odoo es un software de ERP integrado. Cuenta con una versión "comunitaria" de código abierto bajo licencia LGPLv3 y una versión empresarial bajo licencia comercial que complementa la edición comunitaria con características y servicios comerciales y desarrollada por la empresa belga Odoo S.A.

# ¿Cómo activar el modo desarrollador rápidamente?
La extensión para navegadores que todo usuario de Odoo debe tener se llama «Odoo debug» y está disponible, tanto para Google Chrome como para Mozilla Firefox. 
Aquí les dejó los enlaces de descarga:

[Odoo debug para Google Chrome](https://chrome.google.com/webstore/detail/odoo-debug/hmdmhilocobgohohpdpolmibjklfgkbi)

[Odoo debug para Mozilla Firefox](https://addons.mozilla.org/es/firefox/addon/odoo-debug)

La extensión es realmente fácil de usar. Al momento de instalarla, aparecerá el emoji del «mono» con los ojos tapados, indicándonos que no estamos en modo desarrollador. Si hacemos clic sobre el rostro del «mono», el emoji cambiará y aparecerá con la cara descubierta, reflejando que estamos en modo desarrollador y haciendo visible todas las opciones que Odoo muestra en este aspecto.
El modo desarrollador con los «assets» activados, también se puede activar con esta extensión, haciendo doble clic sobre el emoji, lo cual mostrará el rostro de un gorila.

# ¿Cómo instalar Odoo?
Hay varias formas de instalar Odoo, te dejo la referncia en su pág oficial 

[Aquí](https://www.odoo.com/documentation/13.0/administration/install/install.html#windows)

Pero yo en esta guía voy hacer referencia a la instalación en Windows como desarrollador que proporciona una mayor flexibilidad: por ejemplo, permite ejecutar varias versiones de Odoo en el mismo sistema. Bueno para desarrollar módulos, puede usarse como base para la implementación de producción.

**Instalación de origen**
La "instalación" de la fuente se trata realmente de no instalar Odoo y, en su lugar, ejecutarlo directamente desde la fuente.

Finalmente, proporciona un mayor control sobre la configuración del sistema y permite mantener (y ejecutar) más fácilmente múltiples versiones de Odoo una al lado de la otra.
Más➕ info [aquí](https://www.odoo.com/documentation/13.0/administration/install/install.html#setup-install-source)

**Clona el repositorio de Odoo con Git**

Edición de la comunidad:
```
C:\> git clone https://github.com/odoo/odoo.git
```
Enterprise Edition:
```
C:\> git clone https://github.com/odoo/enterprise.git
```
# Oddo con Python
Odoo requiere Python 3.6 o posterior para ejecutarse.
Asegúrese de que la versión sea 3.6 o superior, ya que las versiones anteriores no son compatibles con Odoo.
```
C:\> python --version
```
Verifique también que pip esta instalado
```
C:\> pip --version
```

# postgresql
Odoo utiliza PostgreSQL como sistema de gestión de base de datos.
Descargue e instale PostgreSQL 
[Aquí](https://www.postgresql.org/download/windows/)
Nota : versión compatible: 10.0 y posteriore
Más ➕ Nota importante:
De forma predeterminada, el único usuario es **postgres** pero Odoo prohíbe conectarse como postgres, por lo que debe crear un **nuevo usuario** de PostgreSQL:

 1. Add PostgreSQL’s bin directory (by default: C:\Program Files\PostgreSQL\<version>\bin) to your PATH.
2. Create a postgres user with a password using the pg admin gui:
 - Abra **pgAdmin**.
 - Haga doble clic en el servidor para crear una conexión.
 - Seleccione **Objeto ‣ Crear ‣ Rol de inicio de sesión/grupo**.
 - Introduzca el nombre de usuario en el campo **Nombre de rol** (por ejemplo, ).odoo
 - Abra la ficha Definición e introduzca la contraseña (por ejemplo, ) y, a continuación, haga clic en **Guardar**.
 - Abra la pestaña **Privilegios** y cambie **¿Puede iniciar sesión?** a y **Crear base de datos?**.👌

# virtualenv 
Antes de instalar Odoo en tu PC 🖥 lo primero que debes hacer es crearte un entorno virtual.
```
pip install virtualenv
```
## ¿Cómo crear un entorno virtual con Python?.
Ya tengo mís 🗒 sobre eso:

[Entornos virtuales](https://github.com/javierma73/Entornos-virtuales/blob/main/Entornos-virtuales.md)

Pero puedes consulta referncia ofiacial: 
[virtualenv](https://pypi.org/project/virtualenv)

    

  







 









