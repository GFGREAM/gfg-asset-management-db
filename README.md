# GFG Asset Management DB

[![Estado del Proyecto](https://img.shields.io/badge/Estado-En%20Desarrollo-yellow)](https://github.com/Jazzystic/gfg-asset-management-db)
[![Licencia](https://img.shields.io/github/license/Jazzystic/gfg-asset-management-db)](LICENSE)
[![Hecho por](https://img.shields.io/badge/Autor-Julio%20L%C3%B3pez-blue)](#autor)

Sistema de base de datos centralizada para GFG Real Estate Asset Management, enfocado en el control operativo, financiero y analítico de propiedades hoteleras.

---

## 📌 Objetivo del Proyecto

Consolidar la información clave de operaciones hoteleras en una base de datos relacional moderna, desplegada en Azure, con conectividad a herramientas de análisis (Power BI) y flujos ETL automatizados (n8n). El sistema busca optimizar la disponibilidad de datos, migrando de Excel a una base de datos formal, a saber, PostgreSQL en infraestructura Azure. 

---

## 🧱 Estructura del Repositorio

```bash
gfg-asset-management-db/
├── database/           # Scripts SQL: tablas, migraciones, vistas
├── docs/               # Documentación técnica y estratégica
├── n8n-workflows/      # Workflows ETL (JSON)
├── power-bi/           # Dashboards .pbix y modelos de datos
├── azure-deployment/   # Scripts para provisión en Azure
├── monitoring/         # Configuraciones de monitoreo y alertas
├── security/           # Reglas de acceso, respaldos, auditoría
├── utilities/          # Herramientas auxiliares y transformaciones
├── .gitignore
├── LICENSE
└── README.md
```

---

## 🚀 Estado del Proyecto

| Componente                  | Estado      |
|----------------------------|-------------|
| Infraestructura Azure      | ✅ Completa |
| PostgreSQL Configurado     | ✅ Completo |
| Conectividad pgAdmin/SSL   | ✅ Funcional |
| Estructura de carpetas     | ✅ Implementada |
| Scripts SQL iniciales      | ⏳ En desarrollo |
| Dashboards Power BI        | ⏳ En diseño |
| Automatización n8n         | ⏳ Por configurar |
| Documentación técnica      | ⏳ En progreso |

---

## ⚙️ Guía Inicial

1. **Conexión a la Base de Datos**  
   Usa `pgAdmin4` y conecta con SSL usando las credenciales configuradas en Azure PostgreSQL.

2. **Carga de Estructura**  
   Ejecuta `create_tables.sql` desde la carpeta `database/`.

3. **Automatización**  
   Carga los flujos de `n8n-workflows/` en una instancia n8n en Azure (próximamente).

4. **Visualización**  
   Conecta Power BI a la BD y usa los `.pbix` de `power-bi/`.

5. **Monitoreo y Seguridad**  
   Consulta las carpetas `monitoring/` y `security/` para configuraciones avanzadas.

---

## 📊 Tecnologías utilizadas

- PostgreSQL 17 (Azure Flexible Server)
- Power BI
- n8n (ETL/automatización)
- Azure CLI / Bicep
- GitHub

---

## 👤 Autor

**Julio López**  
Finance Jr Analyst  
GFG Real Estate Asset Management  
📧 julio@gfgam.com.mx

---

## 🧾 Licencia

Este repositorio está bajo la licencia [MIT](LICENSE).
