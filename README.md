# FZ4038-Tarea4-Grupo1
Actividad Tarea 4 Clase Bloomberg – Econometría Financiera FZ4038, EGADE. Grupo 1: Bárbara Martínez Flores (A00919623) y Daniel Mondragón Monroy (A01452205).
# Actividad Tarea 4 Clase Bloomberg – Econometría Financiera (FZ4038)

**Maestría en Finanzas, EGADE Business School, Tecnológico de Monterrey**

- **Profesor:** Dr. Raymundo Díaz Robles
- **Grupo 1:**
  - Bárbara Martínez Flores (A00919623)
  - Daniel Mondragón Monroy (A01452205)
- **Fecha de entrega:** 19 de octubre de 2026

## Descripción

Estimación de ocho regresiones lineales simples (cada acción contra el S&P 500) y de la matriz de correlación de ocho acciones (AAPL, MSFT, NVDA, JPM, GS, XOM, CVX y USO) más el índice, con rendimientos diarios del 2 de enero de 2025 al 12 de octubre de 2026. Los resultados se obtienen en la terminal de Bloomberg (funciones HRA y CORR) y se replican en RStudio con datos de LSEG Workspace para cotejarlos. Como complemento, el análisis se repite con rendimientos intradía de 30 minutos de LSEG (1 de julio al 12 de octubre de 2026) para mostrar el efecto de la frecuencia y del periodo.

El documento está organizado en cinco partes:

1. Datos, periodo y frecuencia.
2. Matriz de correlación: Bloomberg, RStudio y comparación.
3. Regresiones lineales simples contra el S&P 500: Bloomberg, RStudio y comparación, más el complemento intradía.
4. Operaciones en HowMarketsWork de las acciones seleccionadas en Bloomberg, para cada alumno.
5. Preguntas 16.1 a 16.4 del capítulo 16 de Gujarati.

## Archivos

| Archivo | Contenido |
|---|---|
| `Tarea4_Grupo1_FZ4038.Rmd` | Código fuente en R Markdown con el análisis completo (Partes 1 a 5). |
| `Tarea4_Grupo1_FZ4038.html` | Documento final generado a partir del Rmd (Knit). |
| `Tarea4_Grupo1_datosLSEG.xlsx` | Precios de LSEG Workspace. Las hojas `diario` y `30min` contienen las fórmulas de descarga, y las hojas `diario_valores` y `30min_valores` los valores que lee el Rmd. |
| `logo_egade.png` | Logo de EGADE Business School para el encabezado del documento. |
| `bbg_correlacion_config.png` | Configuración de la matriz de correlación en Bloomberg (función CORR). |
| `bbg_correlacion.png` | Matriz de correlación obtenida en Bloomberg. |
| `bbg_hra_*.png` | Regresiones de cada acción contra el S&P 500 en Bloomberg (función HRA): `aapl`, `msft`, `nvda`, `jpm`, `gs`, `xom`, `cvx` y `uso`. |
| `hmw_daniel_posiciones_antes.png` | Portafolio de Daniel Mondragón en HowMarketsWork antes de las operaciones. |
| `hmw_daniel_orden1_venta_uso.png` | Orden de venta parcial de USO. |
| `hmw_daniel_orden2_compra_xom.png` | Orden límite de compra adicional de XOM. |
| `hmw_daniel_orden3_short_gs.png` | Orden de venta en corto de GS. |
| `hmw_daniel_orden4_stop_gs.png` | Orden stop de recompra de protección de GS. |
| `hmw_daniel_ordenes_pendientes.png` | Lista de órdenes pendientes al 13 de octubre de 2026. |

## Cómo reproducir el análisis

1. Descargar todos los archivos en una misma carpeta (en GitHub: **Code → Download ZIP**). El Rmd lee el Excel y las imágenes desde la carpeta en la que se encuentra.
2. Abrir `Tarea4_Grupo1_FZ4038.Rmd` en RStudio o Posit Cloud.
3. Instalar los paquetes necesarios, si no están instalados:
   `install.packages(c("readxl", "quantmod"))`
4. Ejecutar Knit para generar el HTML.
