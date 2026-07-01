# CRM Click24Web — Inmobiliaria

> Sistema de gestión de clientes (CRM) diseñado para inmobiliarias. Una sola página HTML, sin dependencias de build, con sincronización en la nube via Supabase.

![Vista previa](logo.jpg)

---

## 🚀 Funcionalidades

- 📊 **Dashboard** con estadísticas en tiempo real, gráficos y embudo de conversión
- 🏗️ **Pipeline Kanban** con drag & drop por etapas de venta
- 👥 **Gestión de Clientes** con tabla, filtros avanzados y historial de seguimiento
- 🔍 **Búsqueda Inteligente** por nombre, barrio, teléfono, presupuesto, etapa y más
- 📅 **Agenda / Calendario** interactivo con seguimientos y notas de colores
- ⚡ **Registro Rápido** de llamadas y WhatsApp con reprogramación automática
- 💬 **WhatsApp Inteligente** — envío individual y en lote con plantillas personalizables
- ⚙️ **Ajustes** — edición de las 7 plantillas de WhatsApp con variables dinámicas
- 📥 **Exportar a Excel** — CSV compatible con Microsoft Excel en español (UTF-8 + separador `;`)
- 🌙 **Modo Claro / Oscuro** guardado automáticamente
- 📱 **Responsive** — funciona en celular, tablet y desktop
- 📖 **Manual descargable** desde la app (HTML con diseño profesional)
- ☁️ **Sincronización Supabase** + respaldo automático en localStorage

---

## 🛠️ Tecnologías

| Tecnología | Uso |
|---|---|
| HTML5 / CSS3 / JavaScript | Frontend puro, sin frameworks |
| [Supabase](https://supabase.com) | Base de datos en la nube (PostgreSQL) |
| [Chart.js](https://www.chartjs.org/) | Gráficos del Dashboard |
| Google Fonts (Inter) | Tipografía |
| localStorage | Respaldo y persistencia local |

---

## 📁 Estructura del proyecto

```
CRMinmobiliaria/
├── index.html        ← Aplicación principal (HTML + CSS + JS en un solo archivo)
├── deployed.html     ← Copia de producción sincronizada
├── logo.jpg          ← Logo de la empresa
└── README.md         ← Este archivo
```

---

## ⚙️ Configuración de Supabase

1. Creá un proyecto en [supabase.com](https://supabase.com)
2. Creá una tabla llamada `leads` con la siguiente estructura:

```sql
create table leads (
  id           text primary key,
  nombre       text,
  telefono     text,
  localidad    text,
  barrio       text,
  operacion    text,
  tipo_propiedad text[],
  ambientes    text,
  banos        text,
  cochera      text,
  presupuesto_min numeric,
  presupuesto_max numeric,
  moneda       text,
  credito_hipotecario text,
  financiacion text,
  etapa        text,
  origen       text,
  notas        text,
  proximo_contacto date,
  creado_en    date,
  updated_at   timestamptz,
  seguimiento  jsonb
);
```

3. En `index.html`, buscá la sección de configuración de Supabase y reemplazá con tus credenciales:

```js
const SUPABASE_URL = 'https://TU_PROYECTO.supabase.co';
const SUPABASE_KEY = 'TU_ANON_KEY';
```

> Si no configurás Supabase, el CRM funciona igual en **modo local** usando `localStorage`.

---

## 🚀 Uso

No requiere instalación ni build. Simplemente:

```bash
# Opción 1 — Abrir directo en el navegador
Abrí index.html con doble clic

# Opción 2 — Servidor local (recomendado)
npx serve .
# o
python -m http.server 8080
```

---

## 📖 Manual de Usuario

Desde dentro de la app, hacé clic en **📖 Descargar Manual** en el menú lateral. Se descarga un archivo HTML con todas las instrucciones de uso listo para imprimir como PDF.

---

## 🎨 Paleta de colores

| Color | Hex | Uso |
|---|---|---|
| Violeta principal | `#7c3aed` | Primario |
| Violeta claro | `#8b5cf6` | Secundario / hover |
| Verde | `#10b981` | Éxito / Cerrado |
| Rojo | `#ef4444` | Error / Perdido |
| Amarillo | `#f59e0b` | Advertencia |

---

## 📄 Licencia

Uso privado — Click24Web Inmobiliaria.
