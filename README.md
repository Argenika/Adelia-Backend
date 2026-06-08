# Adelia – Backend IA para PYMEs

> Proyecto desarrollado durante las prácticas profesionales en **Andreoli Studio** (Valencia, 2025–2026).
> Código privado por acuerdo con la empresa. Este README documenta la arquitectura, módulos y resultados del proyecto.

 **Producto en producción:** [getadelia.com](https://www.getadelia.com)

---

## ¿Qué es Adelia?

Adelia es un asistente de inteligencia artificial diseñado para pequeñas y medianas empresas. Se instala como plugin modular en WordPress y automatiza tres áreas críticas del negocio: captación de leads, atención al cliente y generación de contenido SEO.

| Resultado | Valor |
|-----------|-------|
|  Tiempo liberado para nuevos negocios | 30% |
|  Incremento en conversión de leads | 20% |
|  Horas ahorradas en contenido SEO/mes | 45h |
|  Disponibilidad del asistente | 24/7 |

---

## Módulos del sistema

###  Adelia Follow Leads
Sistema de seguimiento automático de contactos y leads.
- Genera recordatorios automáticos para el equipo comercial
- Evita que los leads queden sin respuesta
- Aumenta la probabilidad de conversión sin intervención manual
- Integración directa con el CRM de WordPress

###  Adelia iA Chat
Chat inteligente integrado en la web del cliente.
- Captura el lead y guía la venta de forma autónoma
- Filtra posibles clientes antes de que lleguen al equipo humano
- Personalizable por sector (servicios, fábricas, tiendas online)
- Disponible 24/7 con respuestas contextuales mediante API de IA

###  Adelia Blogger
Generador automático de contenido SEO.
- Genera artículos optimizados para posicionamiento en buscadores
- Produce contenido para todo un mes en menos de 30 minutos
- Integración con WordPress para publicación directa

---

## Arquitectura técnica

```
WordPress (frontend + CMS)
│
├── Adelia Core (plugin base)
│   ├── Gestión de módulos
│   ├── Autenticación y licencias
│   └── Panel de administración
│
├── Módulo Follow Leads
│   ├── Captura de formularios → MySQL
│   ├── Sistema de recordatorios automáticos (PHP + WP Cron)
│   └── Notificaciones al equipo comercial
│
├── Módulo iA Chat
│   ├── Widget frontend (JS)
│   ├── Backend PHP → API IA
│   └── Historial de conversaciones → MySQL
│
└── Módulo Blogger
    ├── Interfaz de configuración (WordPress Admin)
    ├── Generación de contenido vía API IA
    └── Publicación automática en WordPress
```

---

## Stack tecnológico

| Tecnología | Uso |
|------------|-----|
| PHP | Lógica backend de los tres módulos |
| MySQL | Base de datos: leads, chats, configuración |
| WordPress | CMS base + sistema de plugins |
| WP Cron | Automatización de tareas periódicas |
| API IA | Generación de respuestas y contenido SEO |
| JavaScript | Widget del chat (frontend) |
| WPBakery | Constructor de páginas del producto |

---

## Mi rol en el proyecto

Desarrollé el backend de Adelia durante mis prácticas de +500 horas en Andreoli Studio (Valencia).

Contribuciones principales:
- Desarrollo de la lógica PHP de los módulos Follow Leads y iA Chat
- Integración de la API de inteligencia artificial para respuestas del chat y generación de contenido
- Diseño y gestión de la base de datos MySQL (leads, historial de conversaciones, configuración por cliente)
- Implementación del sistema de automatización con WP Cron para seguimiento de leads y publicación de contenido
- Testing y despliegue en entorno de producción real con clientes activos

---

## Sectores de aplicación

-  Empresas de servicios
-  Fábricas y manufactura  
-  Tiendas online

---

## Estado del proyecto

 En producción activa  
 Código privado (acuerdo con Andreoli Studio)  
 Sistema modular — cada módulo se contrata y activa de forma independiente

---

## Desarrollado por

**Angelina Lepeshko** — Full-Stack Developer · Valencia  
[github.com/Argenika](https://github.com/Argenika) · [LinkedIn](https://linkedin.com/in/angelina-lepeshko-b9a410329/) · [Portfolio](https://angelinalepeshko.netlify.app)
