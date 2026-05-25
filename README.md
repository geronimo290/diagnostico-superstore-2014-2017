# 🏬 Diagnóstico de Datos — Superstore 2014–2017

Análisis exploratorio end-to-end sobre dataset de ventas de un hipermercado estadounidense. El proyecto simula un entregable real para cliente: un **informe de diagnóstico en PDF** con hallazgos accionables y recomendaciones de negocio.

> **Metodología:** `Python + pandas` → `Canva` para el informe ejecutivo

## 📄 Entregable principal

👉 [Ver informe PDF completo](diagnostico_datos.pdf)

## 📊 Vista previa

![Pagina1](screenshot/diagnostico_data(4).png)
![Pagina2](screenshot/diagnostico_data(3).png)
![Pagina3](screenshot/diagnostico_data(2).png)
![pagina4](screenshot/diagnostico_data(1).png)

## 🎯 Objetivo del análisis

Identificar qué está pasando realmente en el negocio: dónde se gana, dónde se pierde, y qué decisiones concretas pueden mejorar la rentabilidad.

**Período analizado:** 2014–2017  
**Dataset:** 9,994 órdenes · 21 variables · 0 valores nulos  

## 🔍 Hallazgos críticos

| # | Hallazgo | Impacto |
|---|----------|---------|
| 1 | **Pérdida oculta en 10 estados** — Texas acumula -$25k mientras California y NY compensan a nivel regional | Alto |
| 2 | **Tables destruye $17.7k** — vende $206k pero opera con pérdida neta por descuentos del 26% promedio | Alto |
| 3 | **Una orden generó -$6,599** — impresora 3D con 70% de descuento | Alto |
| 4 | **Febrero cae 30–40% sistemáticamente** en los 4 años analizados | Medio |
| 5 | **Copiers es el producto estrella** — 68 órdenes, $55k de ganancia neta | Positivo |
| 6 | **Home Office tiene el mejor margen** (14%) pese a ser el segmento más pequeño | Positivo |

## 💡 Recomendaciones implementadas

1. **Eliminar descuentos > 30% en Furniture** → tope del 15% en toda la categoría
2. **Auditar Texas, Ohio y Pennsylvania** → concentran >60% de pérdidas geográficas
3. **Activar promociones en Febrero** → campaña en Office Supplies (mejor margen)

## 🛠️ Stack técnico

| Herramienta | Uso |
|-------------|-----|
| Python 3.11 | EDA completo, limpieza, análisis bivariado |
| pandas / matplotlib / seaborn | Transformaciones y visualizaciones exploratorias |
| Canva | Informe ejecutivo PDF |
| Dataset | [Superstore Sales — Kaggle](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final) |


## 📓 Sobre el notebook

El notebook `01_EDA.ipynb` cubre:
- Inspección inicial: shape, dtypes, nulos, duplicados
- Limpieza y normalización de columnas
- Análisis univariado: distribuciones, outliers, value counts
- Análisis bivariado: ganancia vs descuento, rentabilidad por región/estado/subcategoría, evolución temporal
- Identificación de órdenes con pérdida extrema
- Exportación de CSV limpio para Power BI

---

**Gerónimo Pautazzo** · [LinkedIn](https://www.linkedin.com/in/geronimo-pautazzo-88900325a/) · [Portfolio completo](https://github.com/geronimo290)
