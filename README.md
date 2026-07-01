# Sistema de Gestión de Garantías

Aplicación Full Stack desarrollada para la gestión de garantías de equipos Lenovo, incluyendo seguimiento de incidencias, control de componentes, dashboards analíticos y generación automática de reportes ejecutivos.

---

## Arquitectura

```text
React (Frontend)
        │
        ▼
.NET 8 REST API
        │
        ▼
SQL Server
```

---

## Funcionalidades Principales

### Gestión de Tickets

- Registro de incidencias
- Búsqueda por serie e inventario
- Actualización de información
- Seguimiento de estados
- Gestión de garantías

### Gestión de Componentes

- Registro de componentes reemplazados
- Historial de cambios
- Relación Ticket-Componente

### Dashboard Analítico

- Total de tickets
- Casos abiertos y cerrados
- Garantías procedentes y no procedentes
- Ranking de componentes
- Casos por mes
- Casos por trimestre
- Tipos de daño

### Reportes

- Exportación CSV
- Exportación Word
- Inclusión automática de gráficos
- Informe ejecutivo automatizado

---

## Tecnologías

### Frontend

- React
- Vite
- Tailwind CSS
- Axios
- Recharts

### Backend

- ASP.NET Core 8
- Entity Framework Core
- SQL Server

### DevOps

- Docker
- Docker Compose
- GitHub

### Testing

- Playwright
- Postman
- Newman

---

## Estructura del Proyecto

```text
GarantiasApp
│
├── Garantias.API
├── garantias-frontend
├── garantias-qa
└── postman
```

---

## Repositorios Relacionados

### Frontend

🔗 https://github.com/GabiProm/garantias-frontend

### Backend

🔗 https://github.com/GabiProm/garantias-api

### QA Automation

🔗 https://github.com/GabiProm/garantias-qa

---

## QA Automation

El proyecto cuenta con pruebas automatizadas para:

### UI Testing

- Crear Ticket
- Buscar Ticket
- Actualizar Ticket
- Agregar Componente
- Dashboard
- Exportación Word

### API Testing

- GET Tickets
- POST Ticket
- GET Ticket por ID
- PUT Ticket
- DELETE Ticket

---

## 📸 Capturas

### 📊 Dashboard
![Dashboard](./screenshots/dashboard-general.PNG)

---

### 📄 Crear Ticket
Apartado para la creación de tickets.

![Crear Ticket](./screenshots/crear.PNG)

---

### 📄 Lista de Tickets
Apartado para la visualización de tickets creados, así como el detalle de cada uno y su eliminación si es necesario.

![lista](./screenshots/lista.PNG)

![Detalle](./screenshots/detalle.PNG)

---

### 📄 Buscar Tickets
Apartado para la búsqueda de tickets.

![Buscar](./screenshots/buscar.PNG)

---

### 📈 Gráficos

![Procede Garantía](./screenshots/procede.PNG)

![Tipo Daño](./screenshots/tipodano.PNG)

![Casos por Mes](/screenshots/casomes.PNG)

![Casos por Trimestre](./screenshots/casotrimestre.PNG)

![Ranking Componentes](/screenshots/ranking.PNG)

---

### 📄 Reporte Word
Resultado de la generación dinámica de un informe en función de los filtros seleccionados en el dashboard.

![Reporte Word](./screenshots/reporte-word.PNG)

---

### 📊 Exportación CSV
Resultado de la exportación de data en función de los filtros aplicados. Incluye resumen, análisis y data completa.

![Export CSV](/screenshots/export-csv.PNG)

---

## Instalación

### Backend

```bash
cd Garantias.API
dotnet restore
dotnet run
```

### Frontend

```bash
cd garantias-frontend
npm install
npm run dev
```

---

## Autor

Henry Gabriel Gómez Gerónimo

Ingeniero Electrónico | Soporte TI N2 | Backend Developer | QA Automation | DevOps Enthusiast