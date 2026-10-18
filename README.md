<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=220&section=header&text=Kevin%20Villeda&fontSize=48&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=Full%20Stack%20Developer%20%7C%20Guatemala&descAlignY=58&descSize=18" width="100%"/>

<a href="https://github.com/Kvilleda089">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=2C5364&center=true&vCenter=true&width=750&lines=Aprendiendo+el+ciclo+completo+del+software+%F0%9F%9A%80;Java+%7C+Spring+Boot+%7C+React+%7C+Angular+%7C+NestJS;Construyendo+proyectos+para+seguir+creciendo+%E2%98%95" alt="Typing SVG" />
</a>

</div>

<br/>

## 👋 Sobre mí

Soy **Kevin Villeda**, Ingeniero en Sistemas y desarrollador full stack, con 4 años como desarrollador. Me gusta construir proyectos propios donde pueda recorrer todo el ciclo de vida del software: desde el análisis y diseño, pasando por el desarrollo, hasta las pruebas y el despliegue.

- 🎓 Ingeniero en Sistemas y Ciencias de la Comunicación — Universidad Mariano Gálvez
- 🎓 Maestría en Informática — Universidad Mariano Gálvez
- 🌱 Aprendiendo constantemente y mejorando con cada proyecto que construyo
- 📫 Contáctame: **struj3884@gmail.com**

<br/>

## 🧰 Stack tecnológico

<div align="center">

<img src="https://skillicons.dev/icons?i=react,angular,ts,js,reactnative,bootstrap,java,spring,nestjs,nodejs,py,fastapi,cs,postgres,mysql,mongodb,redis,docker,kafka,aws,git,idea,vscode&theme=dark" />

</div>

<br/>

<table align="center">
<tr>
<td valign="top" width="50%">

**Frontend**
```
React · Angular · TypeScript
JavaScript · React Native · Bootstrap
```

**Backend**
```
Java (Spring Boot, MicroProfile)
NestJS / Node.js · Python (FastAPI) · C#
```

</td>
<td valign="top" width="50%">

**Bases de datos**
```
PostgreSQL · MariaDB · MySQL
Oracle · MongoDB · Redis
```

**Herramientas & prácticas**
```
Docker · Microservicios · Kafka · BullMQ
AWS S3 · GIT · SCRUM · UML/C4 · JUnit
UiPath (RPA) · Creatio (BPM)
```

</td>
</tr>
</table>

<br/>

## 🚀 Proyectos destacados

<table align="center">
<tr>
<td width="100%">

### 🏟️ Sistema de Reservas de Canchas y Salones

Plataforma para gestionar reservas de dos canchas deportivas y salones de eventos. La pantalla principal muestra el listado de reservaciones con filtros por cliente, hora, fecha y estado.

Backend desplegado en Render · Base de datos en Neon (PostgreSQL)

<img src="https://img.shields.io/badge/CQRS-4B0082?style=for-the-badge" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
<img src="https://img.shields.io/badge/Prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white" />
<img src="https://img.shields.io/badge/NestJS-E0234E?style=for-the-badge&logo=nestjs&logoColor=white" />

<br/><br/>

<a href="https://github.com/Kvilleda089/api-reservation">
  <img src="https://img.shields.io/badge/Ver_repositorio-181717?style=for-the-badge&logo=github&logoColor=white" />
</a>

<br/><br/>

#### 🔧 Despliegue y flujo de trabajo

El proyecto se despliega en **Render** a partir de un `Dockerfile`, con dos ramas conectadas a sus propios servicios (`quality-assurance` para pruebas y `master` para producción), compartiendo una base de datos en **Neon**.

<p align="center">
  <img src="assets/projects/reservation-api/ReservaFacil-Diagrama Despliegue.jpg" width="48%" alt="Configuración de despliegue en Render"/>
  &nbsp;
  <img src="assets/projects/reservation-api/flujo de trabajo.png" width="48%" alt="Flujo de trabajo: develop, quality-assurance y master"/>
</p>

<p align="center">
  <sub><b>Izquierda:</b> configuración del despliegue en Render · <b>Derecha:</b> flujo de ramas de GitHub hacia Render y Neon</sub>
</p>

<br/>

#### 🖥️ Frontend — ReservaFácil (reservation-web)

Interfaz web construida con **Next.js (App Router)**, organizada por features (agenda, auth, dashboard, employee, statistics, client). Maneja el login y la sesión del empleado con `AuthContext`, y protege las rutas según el rol (`COURT_MANAGER`, `ADMINISTRATOR`, `SUPER_ADMINISTRATOR`) con un componente de ruta protegida. Se comunica con la API mediante un cliente Axios con interceptor que agrega el token automáticamente.

<img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" />
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
<img src="https://img.shields.io/badge/TailwindCSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" />
<img src="https://img.shields.io/badge/shadcn%2Fui-000000?style=for-the-badge&logo=shadcnui&logoColor=white" />

<br/><br/>

<a href="https://github.com/Kvilleda089/reservation-web">
  <img src="https://img.shields.io/badge/Ver_repositorio-181717?style=for-the-badge&logo=github&logoColor=white" />
</a>

<br/><br/>

<p align="center">
  <img src="assets/projects/reservation-web/arquitectura_frontend_reservation_web.svg" width="70%" alt="Arquitectura del frontend reservation-web"/>
</p>

<p align="center">
  <sub>Arquitectura del frontend: organización por features, autenticación y rutas protegidas</sub>
</p>

</td>
</tr>
</table>

<br/>

## 🧩 Servicios reutilizables

Microservicios independientes del sistema de reservas. Cada uno se consume por **HTTP con API key**, así que cualquier otro proyecto (incluido el de reservas) puede integrarlos sin tocar su código.

<table align="center">
<tr>
<td width="100%">

### 🔔 Notify Hub

Microservicio de notificaciones por **email y SMS**. Recibe la solicitud por HTTP, la guarda en base de datos, la encola y la envía en segundo plano con reintentos automáticos. Es **multi-tenant**: cada aplicación cliente es un *Project* con sus propias API keys.

- **Idempotencia** con `Idempotency-Key`: reenviar la misma petición no duplica el mensaje.
- **Envío asíncrono** con BullMQ + Redis: 3 intentos con backoff exponencial.
- **Historial de intentos** (`DeliveryAttempt`) con proveedor, estado y error de cada envío.
- **Reenvío manual** de notificaciones enviadas o fallidas.
- **Proveedores intercambiables**: Resend (email) e Infobip o *mock* (SMS); agregar uno nuevo no toca el resto del código.
- Autenticación por **API key** (clientes) y **token de administrador** (gestión de proyectos).

<img src="https://img.shields.io/badge/NestJS-E0234E?style=for-the-badge&logo=nestjs&logoColor=white" />
<img src="https://img.shields.io/badge/CQRS-4B0082?style=for-the-badge" />
<img src="https://img.shields.io/badge/Prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white" />
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" />
<img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" />
<img src="https://img.shields.io/badge/BullMQ-FF6B6B?style=for-the-badge" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
<img src="https://img.shields.io/badge/Jest-C21325?style=for-the-badge&logo=jest&logoColor=white" />

<br/><br/>

<a href="https://github.com/Kvilleda089/notify-hub">
  <img src="https://img.shields.io/badge/Ver_repositorio-181717?style=for-the-badge&logo=github&logoColor=white" />
</a>

<br/><br/>

#### 📐 Diagramas


<p align="center">
  <img src="assets/projects/notify-hub/arquitectura-notify-hub.svg" width="80%" alt="Arquitectura de Notify Hub"/>
</p>
<p align="center">
  <sub>Arquitectura: API, cola con Redis, worker y proveedores de envío</sub>
</p>


<!-- PENDIENTE DIAGRAMA DESPLIEGUES-->

</td>
</tr>
</table>

<br/>

<table align="center">
<tr>
<td width="100%">

### 🧾 PDF Receipts Manager

Servicio centralizado que **convierte HTML en PDF**, le asigna un **número correlativo por proyecto**, lo guarda en **S3** y registra sus metadatos en **PostgreSQL**. Los proyectos consumidores envían el HTML ya armado y reciben el número de documento y una URL prefirmada para descargar el PDF.

- Generación de PDF desde HTML con **WeasyPrint**.
- Numeración independiente por proyecto (`PREFIJO-000001`, `PREFIJO-000002`, …).
- Almacenamiento en **S3** (LocalStack en desarrollo) con URLs prefirmadas de 1 hora.
- Autenticación por **API Key**; en base de datos solo se guarda el hash SHA-256.
- **Aislamiento por proyecto**: un proyecto no puede consultar documentos de otro.
- **Protección contra SSRF**: el HTML solo carga recursos `data:` o de dominios autorizados.
- **CLI** para crear, listar y revocar API Keys.

<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" />
<img src="https://img.shields.io/badge/SQLAlchemy-D71F00?style=for-the-badge&logo=sqlalchemy&logoColor=white" />
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" />
<img src="https://img.shields.io/badge/AWS_S3-569A31?style=for-the-badge&logo=amazons3&logoColor=white" />
<img src="https://img.shields.io/badge/LocalStack-000000?style=for-the-badge" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
<img src="https://img.shields.io/badge/Pytest-0A9EDC?style=for-the-badge&logo=pytest&logoColor=white" />

<br/><br/>

<a href="https://github.com/Kvilleda089/pdf-receipts-manager">
  <img src="https://img.shields.io/badge/Ver_repositorio-181717?style=for-the-badge&logo=github&logoColor=white" />
</a>

<br/><br/>

#### 📐 Diagramas

<p align="center">
  <img src="assets/projects/pdf-receipts-manager/arquitectura.svg" width="80%" alt="Arquitectura de PDF Receipts Manager"/>
</p>
<p align="center">
  <sub>Arquitectura: API, renderer, storage en S3 y base de datos</sub>
</p>
<!-- ESPACIO PARA DESPLIEGUE — PDF Receipts Manager (se integra más adelante) -->

</td>
</tr>
</table>

<br/>

## 📊 Estadísticas

<div align="center">

<img src="https://github-readme-streak-stats.herokuapp.com/?user=Kvilleda089&theme=tokyonight&hide_border=true" />

<br/><br/>

<img src="https://raw.githubusercontent.com/Kvilleda089/Kvilleda089/output/github-contribution-grid-snake.svg" alt="Gráfico de contribuciones animado" />

</div>

<br/>

## 📬 Contacto

<div align="center">

<a href="https://www.linkedin.com/in/kevin-trujillo-2222521a8/">
  <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
</a>
<a href="mailto:struj3884@gmail.com">
  <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" />
</a>

</div>

<br/>

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2c5364,50:203a43,100:0f2027&height=100&section=footer" width="100%"/>

</div>
