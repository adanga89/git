# ¿Qué es GIT? :mailbox:
Software de control de versiones diseñado por **Linus Torvalds**, esto para mantener un buen control y mantenimiento de todos los archivos.

### **Proposito**
Llevar registro de los cambios en archivos y coordinar el trabajo que las personas comparten.

### **En general** :mag_right:
**GIT** es un comparador de texto, este detecta cualquier cadena de texto y busca las diferencias que se encuentran en los archivos.


## _**Iniciando**_ :point_up:
**Instalación**

Descargar el archivo de instalación de acuerdo a tu sistema operativo de la página oficial [Git](https://git-scm.com/) y ejecutalo, o si estas en una distribución de Linux ejecuta el siguiente comando:

```
    Sudo apt-get update Sudo apt-get install git
```

**Verificación de Instalación**

Abre la terminal y ejecuta la siguiente linea de comando

```
    git --version
```

Te saldrá la versión que tienes instalada, por ejemplo:
```
    git version 2.30.1.windows.1
```

## **Configuración del repositorio** :globe_with_meridians:

Para que **Git** funcione, es necesario tener en cuenta el nombre de quien es el que modifica o crea archivos, es por eso que se debe de configurar variables de entorno, así cuando se hagan cambios en los archivos, se vinculará el correo y nombre de las persona. Para esto debememos ejecutar los siguientes comandos:

```
    git config --global user.name 'NombreSinEspacios'
    git config --global user.email 'tucorreo@mail.com'
```

Si utilizas la el identificador **--global**, configura esos dos parametros de forma global, como lo menciona, es decir, en cada repositorio que crees ya no será necesario volver a ingresar esos valores. Por otro lado, si solo requieres que sea en el archivo de configuración local, ejecutas los mismos comandos sin el identificador **--global**

## _**Primeros Pasos**_ :walking:

**Iniciar repositorio GIT**

En la terminal, dirigete a una ruta en donde puedas crear una carpeta.

Ejecuta el siguiente comando:
```
    mkdir [nombreDeLaCarpeta]
```
Ingresa a la carpeta y ejecuta el siguiente comando:
```
    git init
```
El comando de **init**, te iniciará un repositorio de **git**.

**Añadir archivos al área de trabajo**

```
    git add <archivo>
```
Para añadir todos los archivos se ejecuta el siguiente comando.
```
    git add .
```
**Estatus de los archivos**
```
    git status
```

**Ver los cambios generados**
```
    git log
```

**Regresar un cambio de archivo**
```
    git checkout -- <archivo>
```

**Ver la diferencia de los archivos**
```
    git diff -- <archivo>
```
**Guardar cambios**
```
    git commit "[mensaje]"
```
**Ignorar archivos**
Para ignorar archivos que no se requieran en el repositorio se crea un archivo llamado "**.gitignore**"