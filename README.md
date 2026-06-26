# Diagnóstico y Propuestas de Control — Cementos Melón S.A. (Planta La Calera)

Este repositorio contiene el proyecto completamente aislado e independiente de consultoría y propuestas técnicas para la **Planta La Calera (LCA) de Cementos Melón S.A.**, enfocado en el diagnóstico de la red de control de la planta y la formulación de propuestas de modernización y medición de flujo con tecnología **SUPCON**.

---

## 📂 Estructura del Proyecto

El proyecto está organizado con los siguientes archivos clave:

*   **[Minuta_Cementos_Melon.md](Minuta_Cementos_Melon.md):** Minuta técnico-comercial que detalla las problemáticas diagnosticadas (cierre del anillo de fibra óptica, migración de servidores DCS y reemplazo de caudalímetros), junto con la propuesta formal redactada para el cliente.
*   **[dashboard_calera.html](dashboard_calera.html):** Panel interactivo premium que integra la topología de red en formato SVG interactivo, buscador de inventario, minutas y propuestas en una sola interfaz local offline.
*   **[inventario_super_detallado_lca.md](inventario_super_detallado_lca.md) / [inventario_super_detallado_lca.csv](inventario_super_detallado_lca.csv):** Inventario completo auditado desde el plano de red, clasificando 96 unidades físicas de equipos de comunicación, DCS, gateways e instrumentos de campo.
*   **[Plano RedControl LCA_Rev0 (3) (1).dwg](Plano%20RedControl%20LCA_Rev0%20(3)%20(1).dwg):** Plano AutoCAD de control original de la planta.
*   **[Plano_RedControl_LCA.dxf](Plano_RedControl_LCA.dxf) y [textos_extraidos_plano_v2.txt](textos_extraidos_plano_v2.txt):** Archivos intermedios de extracción y auditoría de textos del plano.
*   **[analisis_coordinados_cen.md](analisis_coordinados_cen.md) / [analisis_coordinados_cen.csv](analisis_coordinados_cen.csv):** Análisis complementarios de coordenadas y referencias del plano.

---

## 🛠️ Diagnósticos Clave e Innovaciones

### 1. Robustecimiento de la Red de Control (DCS)
*   **Problemática:** Anillo de fibra óptica actualmente abierto en dos puntos (F012 y F004), lo que elimina la redundancia física y deja la planta expuesta a caídas ante cortes accidentales de fibra.
*   **Propuesta:** Cierre físico del anillo de fibra óptica utilizando la infraestructura existente e instalación de switches industriales SUPCON.
*   **Migración de Servidores:** Actualización de los servidores expertos obsoletos FLSmidth PXP a la plataforma de optimización **SUPCON APC-Cement (Control Predictivo Multivariable)** para optimizar la eficiencia térmica del horno rotatorio.

### 2. Solución para Medición de Flujo de Gas en Condiciones Extremas (Horno de Cemento)
*   **Problemática:** Un caudalímetro de gas E-T-A FC01-CA dañado en una tubería de 1", expuesto a arrastre de cemento (polvo CKD altamente abrasivo), presencia de cloro corrosivo, temperaturas extremas y vibraciones mecánicas.
*   **Propuestas Técnicas SUPCON:**
    *   **Alternativa 1 (Ideal): Caudalímetro de Dispersión Térmica SRF-I.** Medición directa de flujo másico sin partes móviles, con revestimiento de carburo de tungsteno contra la abrasión y sonda retráctil para mantenimiento rápido sin detener el proceso.
    *   **Alternativa 2: Presión Diferencial (CXT + Venturi de Alta Resistencia).** Venturi robusto de pared gruesa con tomas de presión purgadas por aire para evitar la acumulación de polvo de cemento.
    *   **Alternativa 3: Caudalímetro de Vórtice (Vortex SFV-I).** Con sensor piezoeléctrico aislado de alta resistencia a temperaturas y vibraciones.

---

## 💻 Visualización y Uso
Para explorar el proyecto interactivo de forma local y offline, simplemente abra el archivo **[dashboard_calera.html](dashboard_calera.html)** en cualquier navegador web. Encontrará la topología interactiva, el buscador dinámico del inventario de equipos y las minutas comerciales en una interfaz unificada y de alto rendimiento.
