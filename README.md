# Bienvenido

**Aspirante:** Edwar Mauricio Mayorga Llanos  
**Ciudad Origen:** Neiva - Huila  

Este README proporciona las instrucciones para comenzar a trabajar con este proyecto en Python que está alojado en GitHub. Sigue los pasos cuidadosamente y estarás listo para comenzar a utilizar este proyecto.

## 1. Clonar el repositorio desde GitHub

Para empezar, necesitas clonar el repositorio en tu máquina local. Esto se puede hacer utilizando Git, una herramienta de control de versiones. Si no tienes Git instalado, puedes descargarlo desde [aquí](https://git-scm.com/downloads).

Una vez que Git esté instalado, abre una terminal (o Git Bash en Windows) y ejecuta el siguiente comando:

```bash
git clone https://github.com/emmllanitos/test-nequi-python.git
```

## 2. Instalar Python

Este proyecto requiere Python para ejecutarse. Si no lo tienes instalado, puedes descargar la última versión de Python desde [aquí](https://www.python.org/downloads/).

## 3. Crear un entorno virtual de Python

Antes de instalar las dependencias del proyecto, es una buena práctica crear un entorno virtual. Esto permite aislar las dependencias de este proyecto de otras instalaciones de Python en tu sistema.

Para crear un entorno virtual, abre una terminal en el directorio del proyecto clonado y ejecuta el siguiente comando:

```bash
python -m venv venv
```

Este comando creará un nuevo directorio llamado `venv` en el directorio del proyecto, que contendrá el entorno virtual de Python. Para activar el entorno virtual, ejecuta uno de los siguientes comandos, dependiendo de tu sistema operativo: En Windows:

```bash
venv\Scripts\activate
```

En Unix o MacOS:

```bash
source venv/bin/activate
```
Depronto te pida actualizar `pip` pero es opcional.


Ahora estás listo para instalar las dependencias del proyecto.

## 4. Instalar las dependencias del proyecto

Las dependencias necesarias para este proyecto están listadas en el archivo `requirements.txt`. Para instalar estas dependencias, asegúrate de que tu entorno virtual esté activado, luego ejecuta el siguiente comando:
```bash
pip install -r requirements.txt
```


## 5. Ejecutar Jupyter Lab o Visual Studio Code

Este proyecto utiliza notebooks de Jupyter para la visualización y edición de código. Puedes optar por usar Jupyter Lab o Visual Studio Code para abrir estos notebooks.

### Jupyter Lab

Si prefieres usar Jupyter Lab, primero asegúrate de que esté instalado. Si no lo está, puedes instalarlo con el siguiente comando:

```bash
pip install jupyterlab
```

Una vez instalado, puedes iniciar Jupyter Lab con el siguiente comando:
```bash
jupyter-lab
```


Esto abrirá una ventana en tu navegador web con la interfaz de Jupyter Lab, desde la cual puedes abrir los notebooks que se encuentran en el directorio del proyecto.

### Visual Studio Code

Visual Studio Code (VSCode) es otro editor de código que soporta notebooks de Jupyter. Puedes descargar VSCode desde [aquí](https://code.visualstudio.com/).

Una vez instalado VSCode, necesitas instalar la extensión de Python y Jupyter. Puedes hacerlo buscando "Python" y "Jupyter" en el Marketplace de VSCode y  luego  haciendo  clic  en  "Install" en  la  extensión  de  Jupyter. 
 
Con  VSCode  y  la  extensión  de  Jupyter  instalados,  simplemente  abre  el  directorio  del  proyecto  en  VSCode  y  luego  abre  cualquier  notebook.

Si tienes alguna duda, no dudes en escribirme en Linkedin!.

### En cuestion al Paso 5: Completar la redacción del proyecto

El objetivo del proyecto es medir ¿Qué estación de origen y destino se utiliza más?, ¿Qué días son de mayor demanda?, ¿En qué rango de horas se utiliza más el servicio?, ¿Quién usa más el servicio (miembros o ciclistas casuales)? con el proposito de mejorar el servicio en esas estaciones, medir en cuales estaciones estamos haciendo algo mal, beneficiar a los miembros recuerrentes, incentivar a los clientes casuales a volverse miembros.

### Si los datos se incrementaran en 100x.  

- Seguiria funcionando bien la ETL porque esta optimizada.

### Si las tuberías se ejecutaran diariamente en una ventana de tiempo especifica.  
- Seria gasto innecesario porque se estan evaluando periodos anteriores.

### Si la base de datos necesitara ser accedido por más de 100 usuarios funcionales.  
- No se sobrecargaria porque se maneja dwh, entonces no se utiliza bases de datos core.
 
### Si se requiere hacer analítica en tiempo real, ¿cuales componentes cambiaria a su arquitectura propuesta?  
- Cambiar el origen de los datos a un realtime database para poder hacer la extraccion y asi mismo, implementar una ETL en entorno realtime database.
