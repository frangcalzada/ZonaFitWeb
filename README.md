# 🏋️‍♂️ ZonaFit - Proyecto Integral (Consola, Escritorio y Web)

Este proyecto representa la evolución de **ZonaFit**, un sistema de gestión para gimnasios desarrollado en **Java** a través de distintas tecnologías y enfoques. A lo largo del desarrollo se implementaron tres versiones:

1. **Versión de Consola (Java puro)**  
   - Orientada a la práctica de conceptos básicos de **POO en Java**.  
   - Manejo de entidades, colecciones y operaciones CRUD en memoria.  
   - Útil para entender la lógica de negocio sin interfaz gráfica.

2. **Versión de Escritorio (JavaFX / Swing)**  
   - Implementación con interfaz gráfica.  
   - Gestión de clientes, entrenamientos y rutinas desde una aplicación standalone.  
   - Persistencia de datos local (archivos o base de datos simple).

3. **Versión Web (Spring Boot + JSF + PrimeFaces)**  
   - Versión más completa y robusta del sistema.  
   - Orientada a la arquitectura moderna de aplicaciones web.

---

## 🌐 Versión Web: Tecnologías y Arquitectura

La versión **web** de ZonaFit se construyó utilizando un stack de tecnologías modernas:

- **Java 24+**  
- **Spring Boot** → Motor principal para levantar la aplicación y gestionar la configuración.  
- **JSF (Jakarta Faces)** → Framework para la construcción de interfaces web basadas en componentes.  
- **PrimeFaces** → Librería UI que complementa JSF con componentes visuales modernos.  
- **PrimeFlex** → Librería de estilos basada en utilidades CSS (similar a Tailwind).  
- **Maven** → Gestión de dependencias y ciclo de vida del proyecto.  
- **H2 / MySQL** → Base de datos en memoria o persistente para desarrollo/producción.  

---

## ⚙️ Funcionamiento General

La aplicación permite gestionar **clientes, entrenamientos, rutinas y pagos** dentro de un gimnasio.  

- **Capa de Vista (Front-End):**  
  Implementada con **JSF + PrimeFaces**, permitiendo formularios dinámicos, validación y componentes interactivos.

- **Capa de Lógica (Back-End):**  
  Desarrollada con **Spring Boot**, organizando el proyecto en capas:  
  - **Controllers / Beans (JSF ManagedBeans)** → Controladores que gestionan la comunicación entre vista y servicios.  
  - **Services** → Contienen la lógica de negocio.  
  - **Repositories (Spring Data JPA)** → Acceso y persistencia en la base de datos.  
  - **Entities (JPA)** → Modelado de las tablas de la base de datos.

- **Capa de Persistencia (Data):**  
  Uso de **Spring Data JPA** para mapear las entidades del gimnasio en tablas relacionales.

El sistema sigue una arquitectura en **capas**:



---

## 🚀 Ejecución del Proyecto Web

1. Clonar el repositorio:
   git clone https://github.com/frangcalzada/ZonaFitWeb.git
2. Entrar en la carpeta del proyecto:
   cd ZonaFitSpring
3. Ejecutar con Maven
   mvn spring-boot:run
4. Abrir en el navegador
   http://localhost:8080



