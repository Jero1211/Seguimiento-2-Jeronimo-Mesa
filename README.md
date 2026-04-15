# R.I.H.O: Reporte de Incidencias de Hernán Ocazionez

> **Software de Gestión de Servicios de TI (ITSM)** > **Autores:** Jeronimo Mesa Carvajal & Juan Esteban Ospina  
> **Institución:** Ingeniería de Software | 2026

---

## 📝 Introducción
El proyecto **R.I.H.O.** es una solución tecnológica diseñada para la empresa **Hernán Ocazionez S.A.S.** con el fin de transformar la gestión de incidencias técnicas. Implementa un sistema centralizado que garantiza la continuidad del negocio mediante la trazabilidad y la optimización de los procesos de soporte.

## 🚩 Planteamiento del Problema
Actualmente, la organización presenta:
* **Canales Informales:** Dependencia de chats y llamadas que causan pérdida de información.
* **Falta de Trazabilidad:** Dificultad para seguir el estado de los incidentes en tiempo real.
* **Inexistencia de Métricas:** Falta de datos (KPIs) para medir el desempeño del equipo de TI.

## ⚙️ Flujo Operativo (Diagrama de Actividades)
El software sigue un flujo lógico horizontal que asegura que cada reporte sea atendido bajo estándares de calidad.

```mermaid
graph LR
    A((Inicio)) --> B[Reporte de Incidencia]
    B --> C{¿Datos Válidos?}
    C -- No --> B
    C -- Sí --> D[Lógica ITIL]
    D --> E[Dashboard Técnico]
    E --> F[Gestión de Soporte]
    F --> G{¿Resuelto?}
    G -- No --> H[Escalamiento]
    H --> F
    G -- Sí --> I[Cierre y Métricas]
    I --> J((Fin))

    style A fill:#adff2f,stroke:#000,color:#000
    style J fill:#adff2f,stroke:#000,color:#000
    style E fill:#111,stroke:#adff2f,color:#fff
