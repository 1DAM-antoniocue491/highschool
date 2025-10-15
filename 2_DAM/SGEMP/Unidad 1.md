# TEMA 1 — INTRODUCCIÓN A LOS SISTEMAS ERP Y CRM

## 1. Gestión empresarial
- **Definición:** planificación, organización y control de los recursos (dinero, personas, materiales, tiempo…) para alcanzar objetivos.  
- La empresa es un **sistema** que transforma **entradas (recursos)** en **salidas (bienes o servicios)** buscando **beneficio**.  
- Requiere coordinación entre áreas: producción, ventas, compras, finanzas, RRHH…

---
## 2. Conocimientos básicos de gestión empresarial

### 🔹 Planificación y gestión del personal (RRHH)
- **Tradicional:** administración (nóminas, contratos, ausencias) y legalidad (Seguridad Social, riesgos laborales).  
- **Moderno:** el personal es un **activo estratégico** → se gestiona el **talento** (HCM – Human Capital Management).  
- **Ciclo HCM:**  
  - **Atracción:** reclutamiento y selección.  
  - **Desarrollo:** formación, evaluación, carrera profesional.  
  - **Retención:** mantener empleados clave.  
- Surgen los **HRIS** (Human Resources Information Systems): automatizan procesos y liberan RRHH para tareas estratégicas.  

---
### 🔹 Marketing y ventas
- **Marketing:** atraer clientes (investigación, publicidad).  
- **Ventas:** convertirlos en ingresos.  
- Aquí actúa el **CRM**.  
- **Embudo de ventas:** recorrido del cliente desde el primer contacto hasta la compra.

---
### 🔹 Plan estratégico
- Define **misión**, **visión**, **objetivos** y **recursos**.  
- Ejemplo: “Ser líder en el sector”, “Aumentar ventas un 15%”.  
- Toda empresa planifica; no improvisa.

---
### 🔹 Gestión de operaciones
- Asegura que la empresa **produce con calidad y bajo coste**.  
- En software surge el concepto **DevOps** → unión de desarrollo (Dev) y operaciones (Ops) para automatizar, colaborar y entregar software de forma continua (**CI/CD**).

---
### 🔹 Sistema de producción
- **En masa:** grandes volúmenes, eficiencia, automatización.  
- **Por encargo:** producción personalizada, flexibilidad.  
- **Mixta:** combinación de ambas.  
- El **ERP** adapta su planificación según el tipo de producción.

---
### 🔹 Logística y cadena de suministro
- Controla transporte, almacenes y distribución.  
- Si un proveedor falla, se interrumpe toda la cadena.  
- Muy importante en **e-commerce** y **retail**.

---
### 🔹 Entorno empresarial
- Factores externos: competencia, leyes, economía, tecnología…  
- Las empresas deben **adaptarse al entorno** (pandemia, guerras, etc.).

---
## 3. Evolución de la informática de gestión empresarial

| Época | Características |
|-------|------------------|
| **1960s** | Mainframes, contabilidad básica |
| **1970s** | MRP (Material Requirement Planning) |
| **1980s** | MRP II (Manufacturing Resource Planning) |
| **1990s** | Nacimiento de los **ERP integrados** |
| **2000s** | Internet → ERP/CRM web, integración con e-commerce y banca online |
| **Actualidad** | **Cloud ERP**, movilidad, IA, automatización (RPA), integración total |

**Tendencias:**
- Modelo **cloud** (pago mensual, sin servidores propios).  
- **Movilidad:** apps conectadas al ERP.  
- **IA:** predicción de ventas, chatbots, análisis de sentimiento.  
- **BI (Business Intelligence):** integración con Power BI, Tableau…  

---
## 4. Sistemas ERP (Enterprise Resource Planning)

### 🔹 Concepto
Software que **integra todos los procesos clave** de la empresa en un solo sistema:
- Finanzas
- Compras
- Producción
- Inventario
- Ventas
- Recursos Humanos
- Logística, proyectos, mantenimiento…

Evita duplicidades, errores y retrasos → **una única base de datos.**

### 🔹 Ejemplo
Cliente compra online → ERP actualiza stock, factura, avisa logística, registra ingreso → todo automático.

---
### 🔹 ERPs actuales
- **Grandes empresas:** SAP, Oracle ERP, Microsoft Dynamics 365.  
- **PYMEs:** Odoo, Dolibarr, ERPNext, Tryton.  
- **SaaS (Cloud):** NetSuite, SAP S/4HANA Cloud, Odoo.sh.  

**Ventajas del ERP en la nube:**
- Sin servidores propios.  
- Actualizaciones automáticas.  
- Acceso remoto.  
- Menor dependencia del IT interno.  

**Desventajas:**
- Requiere Internet.  
- Coste recurrente.  
- Menor control sobre datos.

---
### 🔹 Criterios de elección
- Tamaño de empresa y transacciones.  
- Coste de licencias y mantenimiento.  
- Soporte local y “partners”.  
- Facilidad de personalización.  
- Compatibilidad legal (fiscal y contable).  

---
## 5. Sistemas CRM (Customer Relationship Management)

### 🔹 Concepto
Software para **gestionar la relación con clientes y prospectos**.  
**Objetivo:** mejorar ventas, fidelización y servicio.

**Funciones:**
- Gestión de contactos y cuentas.  
- Automatización de marketing (emails, campañas).  
- Atención al cliente (tickets).  
- Informes de ventas y comportamiento.  
- Oportunidades / pipeline de ventas.

**Diferencia con ERP:**  
- **ERP:** procesos internos (producción, finanzas).  
- **CRM:** relación externa (clientes, ventas, marketing).  
- Integrados, evitan duplicidades y errores.

### 🔹 CRMs actuales
- **Líderes:** Salesforce, HubSpot, Zoho CRM.  
- **PYMEs:** Odoo CRM, Pipedrive.  

---
## 6. Arquitectura de un sistema ERP-CRM

### 🔹 ¿Por qué unirlos?
- ERP “no sabe” de clientes; CRM “no sabe” de facturación.  
- Integración → coherencia, automatización, sin duplicidades.

### 🔹 Capas del sistema
1. **Interfaz de usuario:** parte visible (web, app).  
2. **Lógica de negocio (módulos):** reglas y procesos empresariales (ventas, contabilidad…).  
3. **Capa de integración / API:** conecta ERP-CRM con otros sistemas (tiendas online, bancos…).  
4. **Base de datos central:** guarda toda la información compartida.  
5. **Servicios de soporte:** reportes, auditoría, workflows, seguridad.

**Analogía:** edificio → interfaz (planta alta), módulos (máquinas), API (conductos), base de datos (sótano), servicios (cimientos).

---
### 🔹 Tipos de arquitectura

| Tipo | Descripción | Ventajas / Inconvenientes |
|------|--------------|---------------------------|
| **Monolítica** | Todo en una sola aplicación. | + Simplicidad / - Poco flexible, difícil de escalar. |
| **SOA (Service-Oriented Architecture)** | Colección de servicios empresariales amplios conectados por un **ESB (Enterprise Service Bus)**. | + Reutilización / - Dependencia si comparten base de datos. |
| **Microservicios** | Servicios pequeños y autónomos, cada uno con su propia base de datos. | + Escalabilidad, independencia tecnológica / - Mayor complejidad de gestión. |
| **Orientada a eventos** | Comunicación asíncrona mediante eventos y colas de mensajes. | + Desacoplamiento / ideal para integrar ERP on-premise con CRM en la nube. |
