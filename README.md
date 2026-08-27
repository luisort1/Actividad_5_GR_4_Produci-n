# Actividad 5 - Analítica de Órdenes de Producción

## Autores

- Laila Tatiana Cardenas Guerrero
- Luis Eduardo Ortega Montes

## Asignatura

Fundamentos de Programación para Analítica de Datos

Universidad Central

---

# Descripción del Caso

La organización requiere identificar las órdenes de producción que no cumplen los criterios establecidos para su cierre y liberación.

El análisis integra información operacional proveniente de SAP relacionada con:

- Órdenes de producción.
- Consumos reales.
- Recetas estándar.
- Conversiones de unidades.
- Tolerancias de peso.
- Tolerancias de consumo.
- Reglas especiales de negocio.

---

# Pregunta de Negocio

¿Qué órdenes deben reportarse por no cumplir los criterios de cierre y liberación?

---

# Unidad de Análisis

Orden de producción.

---

# Usuarios Objetivo

- Líder de Producción.
- Analista de Costos.

---

# Objetivo General

Desarrollar una solución analítica reproducible en Python que permita validar órdenes de producción mediante la comparación entre:

- Consumos esperados.
- Consumos reales.
- Cumplimiento de tolerancias de peso.
- Reglas de parametrización.

Generando alertas y recomendaciones para apoyar las decisiones de producción y costos.

---

# Estructura del Proyecto

<img width="3245" height="2268" alt="image" src="https://github.com/user-attachments/assets/e136814b-a087-4b92-947c-2d75a1d322c8" />

# Flujo General del Análisis 
1. Carga de archivos.
2. Validación de estructura.
3. Normalización de datos.
4. Validación de reglas de negocio.
5. Consolidación de movimientos SAP.
6. Construcción de órdenes.
7. Construcción del detalle orden-receta.
8. Conversión de unidades.
9. Comparación esperado vs real.
10. Evaluación de tolerancias.
11. Identificación de componentes no parametrizados.
12. Pruebas internas.
13. Construcción de indicadores.
14. Generación de gráficos.
15. Generación de informe HTML.
16. Exportación de resultados.

# Fuentes de Datos El análisis utiliza ocho fuentes:

# Validaciones Implementadas

## Estructura
- Columnas obligatorias.
- Archivos vacíos.
- Separación correcta de columnas.
  
## Calidad de Datos
- Registros duplicados.
- Llaves duplicadas.
- Códigos obsoletos.
  
## Negocio 
- Existencia de recetas.
- Existencia de conversiones.
- Consistencia de movimientos SAP.
- Componentes no parametrizados.
  
## Controles Internos - Órdenes esperadas. 
- Detalle esperado.
- Conversión correcta de unidades.
- Pesos no negativos.
- Validación de movimientos de revisión.

# Indicadores Generados 

# Resultados Generados El proceso produce: 
- Resumen por orden.
- Detalle completo.
- Detalle de novedades.
- Control de peso.
- Componentes no parametrizados.
- Indicadores ejecutivos.
- Gráficos interactivos.
- Informe HTML.
- Archivo ZIP consolidado.
  
# Principales Supuestos 
- La unidad de análisis corresponde a una orden de producción.
- Las recetas representan el consumo estándar esperado.
- Las conversiones parametrizadas son correctas.
- Los movimientos SAP se clasifican según las reglas definidas.

# Limitaciones 
- El análisis depende de la calidad de la parametrización.
- Los componentes sin receta se reportan como advertencia.
- Nuevas unidades de medida requieren actualización de la tabla de conversiones.
- Nuevos movimientos SAP requieren parametrización.

# Declaración de Uso de Inteligencia Artificial
Durante el desarrollo del proyecto se utilizaron herramientas de Inteligencia Artificial Generativa como apoyo para:
Revisión de código.
Documentación.
Optimización de estructura.
Todas las decisiones analíticas, validaciones de negocio, interpretación de resultados y conclusiones finales fueron verificadas por los autores.
