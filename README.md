# Proyecto: Spring Microservices para Principiantes
Este proyecto es una arquitectura de microservicios desarrollada en Spring Boot. Permite gestionar servicios de configuración, cursos, estudiantes, registro (Eureka) y una puerta de enlace (Gateway) para el manejo de peticiones dentro de un ecosistema distribuido.

## Estructura del Proyecto
- microservice-config : Servicio de configuración centralizada.
- microservice-course : Servicio para la gestión de cursos.
- microservice-eureka : Servicio Eureka de descubrimiento y registro.
- microservice-gateway : Puerta de enlace que enruta las solicitudes hacia los microservicios.
- microservice-student : Servicio para la gestión de estudiantes.
Cada carpeta contiene su propio archivo pom.xml , código fuente (carpetas src/main y src/test ), y archivos de configuración Maven/Wrapper.

## Requisitos previos
- Java 11+
- Maven 3.8+
- IDE compatible (IntelliJ IDEA, Eclipse, VSCode, etc.)
## Cómo ejecutar los servicios
1. Clonar el repositorio:
   
   ```
   git clone https://github.com/
   Jonathan-Prime/
   Proyect-Microservices-Spring.git
   ```
2. Entrar en la carpeta del proyecto:
   
   ```
   cd Proyect-Microservices-Spring
   ```
3. Levantar los microservicios:
   
   Abre una terminal para cada servicio y ejecuta en la carpeta correspondiente:
   
   ```
   mvn spring-boot:run
   ```
   (Inicia primero microservice-config , luego microservice-eureka , seguidos de los demás.)
## Notas adicionales
- Puedes modificar archivos de configuración en microservice-config para cambios centralizados.
- El registro de servicios se realiza automáticamente a través de Eureka.
- Las rutas y reglas del gateway pueden personalizarse en microservice-gateway .
