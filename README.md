# GFG Asset Management DB

[![Estado](https://img.shields.io/badge/Estado-Semana%201%20de%2024-yellow)](https://github.com/GFGREAM/gfg-asset-management-db)
[![Avance](https://img.shields.io/badge/Avance-4%25%20Completado-orange)](https://github.com/GFGREAM/gfg-asset-management-db)
[![Milestone](https://img.shields.io/badge/Milestone-Database%20Core-success)](https://github.com/GFGREAM/gfg-asset-management-db)
[![Cronograma](https://img.shields.io/badge/Cronograma-6%20días%20adelantado-brightgreen)](https://github.com/GFGREAM/gfg-asset-management-db)
[![Budget](https://img.shields.io/badge/Budget-77%25%20ahorro-brightgreen)](https://github.com/GFGREAM/gfg-asset-management-db)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)
[![Autor](https://img.shields.io/badge/Autor-Julio%20López-blue)](#autor)

Sistema de base de datos centralizada para GFG Real Estate Asset Management, enfocado en el control operativo, financiero y analítico de propiedades hoteleras.

---

## 📌 Objetivo del Proyecto

Consolidar la información clave de operaciones hoteleras en una base de datos relacional moderna, desplegada en Azure, con conectividad a herramientas de análisis (Power BI) y flujos ETL automatizados (n8n). El sistema busca optimizar la disponibilidad de datos, migrando de Excel a una base de datos formal, a saber, PostgreSQL en infraestructura Azure.

---

## 🧱 Estructura del Repositorio

```bash
gfg-asset-management-db/
├── database/           # Scripts SQL: tablas, migraciones, vistas
│   ├── schemas/        # ✅ Esquemas organizacionales implementados
│   ├── migrations/     # Scripts de migración y actualizaciones
│   └── sample-data/    # ✅ Datos de prueba con KPIs validados
├── docs/               # Documentación técnica y estratégica
│   ├── images/         # ✅ Screenshots de progreso y milestones
│   ├── progress/       # ✅ Reportes de avance por semana
│   └── technical/      # Documentación técnica detallada
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

## 🎯 Milestone Actual: Database Core Operational

**📅 Completado**: Agosto 7, 2025  
**⏰ Status**: 6 días adelantado al cronograma de 24 semanas  
**💰 Budget**: $72/mes vs $320 presupuestado (77% de ahorro)  
**📈 Progreso**: Semana 1 de 24 completada exitosamente

### ✅ Logros Alcanzados (~17% Fase 1, ~4% proyecto total)

#### Infraestructura y Arquitectura
- [x] **Azure PostgreSQL 17.6** desplegado y optimizado para BI workloads
- [x] **SSL/TLS security** implementado con conexión segura
- [x] **Resource optimization** con 77% de ahorro en costos
- [x] **Backup automático** y recovery systems activos

#### Implementación de Base de Datos
- [x] **6 esquemas organizacionales** creados:
  - `security` - Usuarios, roles y auditoría
  - `core` - Hoteles y datos principales  
  - `finance` - P&L, weekly pace, forecasting
  - `analytics` - KPIs, benchmarking, análisis de mercado
  - `integrations` - Light House, Demand 360, Costar
  - `automation` - Workflows N8N, ETL processes
- [x] **Sistema de usuarios de 4 niveles** con permisos granulares
- [x] **Tablas principales implementadas** con validaciones de negocio
- [x] **Motor de cálculo automático** para KPIs financieros
- [x] **Sistema de auditoría completo** con logging de todas las operaciones

#### Validación de Datos y KPIs
- [x] **3 hoteles de ejemplo** con datos realistas insertados
- [x] **Cálculos automáticos validados**:
  - Occupancy rates: 65% - 90%
  - ADR (Average Daily Rate): $1,113 - $1,571
  - RevPAR (Revenue per Available Room): $791 - $1,410
  - EBITDA Margins: 51% - 61%
- [x] **Vista calculada** `weekly_pl_calculated` operativa
- [x] **Comparativas ACTUAL vs FORECAST** funcionando

---

## 🚀 Estado del Proyecto por Fases

### 📊 Fase 1: Infraestructura y Arquitectura Core (Semanas 1-6) - EN PROGRESO

| Componente | Estado | Progreso | Notas |
|------------|--------|----------|-------|
| Infraestructura Azure | ✅ Completa | 100% | PostgreSQL 17.6 operativo |
| PostgreSQL Configurado | ✅ Completo | 100% | SSL, backups, optimization |
| Conectividad pgAdmin/SSL | ✅ Funcional | 100% | Conexión segura establecida |
| Esquemas y Tablas Core | ✅ Completado | 100% | 6 esquemas, tablas principales |
| KPIs Automáticos | ✅ Operativo | 100% | Vista calculada funcionando |
| Deploy N8N en VM | ⏳ Pendiente | 0% | Semana 2-3 |
| Workflow Excel → PostgreSQL | ⏳ Pendiente | 0% | Semana 3-4 |
| Sistema de Alertas | ⏳ Pendiente | 0% | Semana 4-5 |
| Validación Final Fase 1 | ⏳ Pendiente | 0% | Semana 6 |

**Progreso Fase 1**: 5 de 9 componentes completados (56%)

### 📈 Fase 2: Módulos Operativos e Integración BI (Semanas 7-12) - PENDIENTE

| Componente | Estado | Progreso | Notas |
|------------|--------|----------|-------|
| P&L Semanal Avanzado | ⏳ No iniciado | 0% | Módulos complejos P&L |
| Weekly Pace con Históricos | ⏳ No iniciado | 0% | Migración datos históricos |
| Validaciones de Negocio | ⏳ No iniciado | 0% | Reglas complejas validación |
| Conexión PostgreSQL-Power BI | ⏳ No iniciado | 0% | Integración nativa |
| Dashboards Analíticos | ⏳ No iniciado | 0% | Dashboards core BI |
| Dashboard Ejecutivo | ⏳ No iniciado | 0% | Vista C-level |
| Importación Datos Históricos | ⏳ No iniciado | 0% | Migración completa |
| Documentación Operativa | ⏳ No iniciado | 0% | Manuales técnicos |

**Progreso Fase 2**: 0 de 8 componentes completados (0%)

### 🔗 Fase 3: Integraciones Externas y Automatización (Semanas 13-18) - PENDIENTE

| Componente | Estado | Progreso | Notas |
|------------|--------|----------|-------|
| Integración Light House | ⏳ No iniciado | 0% | Pricing y ranking automático |
| Dashboards de Mercado | ⏳ No iniciado | 0% | Análisis competitivo |
| Extracción Costar (PDF) | ⏳ No iniciado | 0% | Procesamiento automático |
| Benchmarking Competitivo | ⏳ No iniciado | 0% | Market intelligence |
| Automatización Demand 360 | ⏳ No iniciado | 0% | Monthly OTB automático |
| Forecasting Básico | ⏳ No iniciado | 0% | Modelos predictivos |
| Alertas de Desviaciones | ⏳ No iniciado | 0% | Sistema proactivo |

**Progreso Fase 3**: 0 de 7 componentes completados (0%)

### 🤖 Fase 4: Capacidades Avanzadas y Go-Live (Semanas 19-24) - PENDIENTE

| Componente | Estado | Progreso | Notas |
|------------|--------|----------|-------|
| Azure Machine Learning | ⏳ No iniciado | 0% | Configuración AI/ML |
| Análisis de Sentimiento | ⏳ No iniciado | 0% | Reviews automático |
| Detección de Anomalías | ⏳ No iniciado | 0% | Alertas predictivas |
| Dashboards por Propietario | ⏳ No iniciado | 0% | Personalización individual |
| Power BI App Móvil | ⏳ No iniciado | 0% | Aplicación móvil |
| Sistema de Notificaciones | ⏳ No iniciado | 0% | Push notifications |
| Capacitación Diferenciada | ⏳ No iniciado | 0% | Training por rol |
| Go-Live Controlado | ⏳ No iniciado | 0% | Implementación producción |
| Monitoreo Post Go-Live | ⏳ No iniciado | 0% | Soporte operativo |

**Progreso Fase 4**: 0 de 9 componentes completados (0%)

### 📊 Resumen General del Proyecto

| Fase | Componentes Totales | Completados | Progreso Fase | Contribución al Proyecto |
|------|-------------------|-------------|---------------|-------------------------|
| **Fase 1** | 9 | 5 | 56% | ~4% del total |
| **Fase 2** | 8 | 0 | 0% | ~0% del total |
| **Fase 3** | 7 | 0 | 0% | ~0% del total |
| **Fase 4** | 9 | 0 | 0% | ~0% del total |
| **TOTAL** | **33** | **5** | **15%** | **4% COMPLETADO** |

---

## ⚙️ Guía Inicial

### 1. Conexión a la Base de Datos
Usa `pgAdmin4` y conecta con SSL a:

Server: gfg-postgresql-server-2025.postgres.database.azure.com
Database: gfg_asset_management
Port: 5432
SSL: Required

### 2. Carga de Estructura
Ejecuta los scripts desde `database/schemas/`:

# Script principal con esquemas y tablas
database/schemas/01-complete-setup.sql

# Datos de ejemplo para validación
database/sample-data/hotels-example.sql

### 3. Validación de KPIs
Ejecuta esta query para verificar cálculos automáticos:

SELECT 
    h.codigo, h.nombre, pl.tipo,
    pl.occupancy_rate, pl.adr, pl.revpar, pl.ebitda_margin
FROM finance.weekly_pl_calculated pl
JOIN core.hoteles h ON pl.hotel_id = h.id
ORDER BY h.codigo, pl.tipo;

### 4. Próximos Pasos
- **Semana 2**: Setup N8N VM en Azure
- **Semana 3**: Primer workflow Excel → PostgreSQL
- **Semana 4**: Integración Power BI nativa

---

## 🎯 Roadmap - Próximos Milestones

### Semana 2-6: Completar Fase 1 (Target: ~25% proyecto total)
- [ ] Deploy Azure VM para N8N
- [ ] Primer ETL workflow operativo
- [ ] Sincronización Excel → PostgreSQL
- [ ] Validaciones automáticas de datos

### Semana 7-12: Power BI Integration (Target: ~50% proyecto total)
- [ ] Conexión nativa PostgreSQL → Power BI
- [ ] Dashboards diferenciados por rol
- [ ] Actualización automática de datos
- [ ] Mobile app configuration

### Semana 13-24: External Integrations & Go-Live (Target: 100%)
- [ ] Light House integration (pricing, ranking)
- [ ] Demand 360 automation (Monthly OTB)
- [ ] Costar data processing (market analysis)
- [ ] AI/ML forecasting capabilities
- [ ] Go-live controlado y capacitación

---

## 📊 Tecnologías utilizadas

- **PostgreSQL 17** (Azure Flexible Server)
- **Power BI** (Business Intelligence)
- **n8n** (ETL/automatización)
- **Azure CLI / Bicep** (Infrastructure as Code)
- **GitHub** (Version control & documentation)

---

## 📚 Documentación Adicional

- Milestone Week 01 Report: `docs/progress/milestone-week-01.md`
- Database Setup Guide: `docs/technical/database-setup.md`
- KPI Calculation Documentation: `docs/technical/kpi-calculations.md`
- Security & Access Control: `docs/technical/security-setup.md`

---

## 👤 Autor

**Julio López**  
Finance Jr Analyst  
GFG Real Estate Asset Management  
📧 julio@gfgam.com.mx  
🐙 [@Jazzystic](https://github.com/Jazzystic)

---

**Última actualización**: Agosto 7, 2025 | **Próxima review**: Agosto 14, 2025
