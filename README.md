# Aula Beckhoff

Este proyecto utiliza **Docker** y **Docker Compose** para desplegar un entorno preconfigurado. Sigue los pasos a continuación para clonar el repositorio, configurar el entorno y gestionar los contenedores.

---

## Requisitos Previos

1. **Instalar Docker**: Asegúrate de tener instalado Docker en tu sistema. Puedes descargarlo desde [Docker Official Site](https://www.docker.com/).
2. **Instalar Docker Compose**: Docker Desktop ya incluye Docker Compose. En caso contrario, instálalo siguiendo [esta guía](https://docs.docker.com/compose/install/).
3. **Permisos de Usuario**:
   - Asegúrate de que tu usuario tiene permisos para usar Docker. Para ello, ejecuta:
     ```bash
     sudo usermod -aG docker $USER
     ```
   - Después, cierra sesión y vuelve a iniciar sesión para aplicar los cambios.

---

## Pasos para Ejecutar el Proyecto

1. Clona este repositorio:
   ```bash
   git clone <URL_DEL_REPOSITORIO>
   cd <NOMBRE_DEL_REPOSITORIO>
  ```
r el Proyecto

1. Clona este repositorio:
   ```bash
   git clone <URL_DEL_REPOSITORIO>
   cd <NOMBRE_DEL_REPOSITORIO>
  ```
2. Accede a la carpeta src:

```bash
cd src
  ```
3. Levanta los contenedores usando Docker Compose:

```bash
docker compose up
```
#### Si deseas ejecutar los contenedores en segundo plano (sin mostrar logs), usa:
```bash
docker compose up -d
```

Espera a que los contenedores se inicien correctamente.

4. Detener los Contenedores
Para detener y eliminar los contenedores, redes y volúmenes creados por Docker Compose, usa:

```bash
docker compose down
```

## Notas Adicionales
Si encuentras problemas al levantar los contenedores, verifica que los servicios de Docker estén corriendo:
```bash
systemctl status docker
```

Para inspeccionar los logs de los contenedores mientras están ejecutándose, utiliza:
```bash
docker compose logs -f
```
