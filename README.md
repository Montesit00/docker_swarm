# Parcial Docker-Swarm-Rest-Soap
## Alumno: Montellano Marcos
```markdown
Este proyecto contiene una aplicación que utiliza servicios SOAP y REST, implementados con Node.js y MySQL, y se ejecuta en contenedores Docker. La aplicación consulta y muestra datos de alumnos a través de servicios SOAP y REST.

## Configuración del Entorno

1. **Clonar el Repositorio:**
   ```bash
   git clone <URL del repositorio>
   cd <nombre-del-repositorio>
```
El resto de los pasos esta en el archivo pasos.txt. Esos son los pasos que hice para realizar este examen
#### Imagenes
* Base de datos - imagen: parcial_swarm_basededatos
* Servicio Rest - imagen: parcial_swarm_rest_service
* Servicio Soap - imagen: parcial_swarm_soap_service 
* Front - imagen: parcial_swarm_front_service

### Hacer Docker Build

	1)- docker build -t parcial_swarm_basededatos ./bd
 	2)- docker build -t parcial_swarm_rest_service ./rest_service
  	39- docker build -t parcial_swarm_soap_service ./soap_service
   	4)- docker build -t parcial_swarm_front_service ./front

### Luego inicializar Docker Swarm

	1)- docker swarm init
	2)- docker stack deploy -c docker-compose.yml parcial_swarm
