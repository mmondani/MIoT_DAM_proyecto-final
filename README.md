MIoT - DAM: Trabajo Final
=======================

## Primeros pasos

### Instalar las dependencias

Para correr este código es necesario contar con `Docker` y `Docker-compose` instalados. Para instalarlos en Linux, se pueden seguir los pasos del siguiente [artículo](https://www.gotoiot.com/pages/articles/docker_installation_linux/).


Por otra parte es necesario contar con `Node.js`, `Angular` y `Ionic`.

`Node` se puede desccargar desde el siguiente [link](https://nodejs.org/es/).

Una vez instalado Node, también instala el manejador de paquetes `npm`. Mediante esta utilidad, se debe instalar `Angular` ejecutando el siguiente comando:

```
npm install -g @angular/cli 
```

Finalmente, para instalar Ionic, se procede de manera similar, usando este comando:

```
npm install -g @ionic/cli
```

### Descargar el código

Para descargar el código se debe ejecutar el siguiente comando:

```
git clone https://github.com/mmondani/MIoT_DAM_proyecto-final.git
```

Una vez hecho esto, se deben descargar los submódulos del proyecto. Moverse a la carpeta raiz del repositorio clonado y ejecutar el siguiente comando:

```
git submodule update --init --recursive --remote
```

### Ejecutar el backend

Para ejecutar el backend se debe correr el siguiente comando desde la carpeta `backend` dentro del proyecto:

```
docker-compose up
```

En caso de que arroje algún error relacionado a la base de datos, se recomienda detener los contenedores (presionando `Ctrl+C` en la terminal donde se ejecutó el comando docker-compose up) y volver a ejecutar el comando docker-compose up


### Ejecutar el frontend

Para correr el frontend, ubicándose dentro de la carpeta `frontend`, ejecutar los siguientes comandos:

```
npm install
ionic serve --lab
```

## Detalles de implementación

### Frontend

Para ver ver una explicación detallada de la implementación del frontend, consultar el siguiente [link](https://github.com/mmondani/MIoT_DAM_Proyecto_Ionic).

### Backend

Para ver ver una explicación detallada de la implementación del backend, consultar el siguiente [link](https://github.com/mmondani/MIoT_DAM_Backend).