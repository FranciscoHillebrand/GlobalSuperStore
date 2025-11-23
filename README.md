# 🌍 Global Super Store: Análisis Operativo con Google Sheets

![Status](https://img.shields.io/badge/Status-Finalizado-success?style=for-the-badge)
![Tool](https://img.shields.io/badge/Herramienta-Google%20Sheets%20%2F%20Excel-217346?style=for-the-badge&logo=google-sheets&logoColor=white)

## 📖 Descripción del Proyecto

**Global Super Store**, un gigante del comercio electrónico, buscaba optimizar su eficiencia operativa tras una larga trayectoria en el mercado. Como **Data Analyst**, fui encargado de descifrar la operación empresarial analizando los pedidos realizados a nivel mundial entre el **1 de enero de 2013 y el 31 de diciembre de 2014**.

El desafío principal fue realizar el ciclo completo de análisis de datos (**ETL, Modelado, Análisis Exploratorio y Visualización**) utilizando exclusivamente herramientas de hojas de cálculo (Google Sheets), demostrando que la profundidad del análisis no depende de la complejidad del software, sino de la metodología aplicada.

---

## 🎯 El Desafío de Negocio

La gerencia planteó interrogantes clave para entender la salud del negocio:
* ¿Cuál es la **tendencia** de las ventas? ¿Existe estacionalidad?
* ¿Cómo es el rendimiento comparativo **año tras año** (YoY)?
* ¿Qué **productos o categorías** impulsan el negocio y cuáles generan pérdidas?

Para responder a esto, fue necesario estructurar los datos entendiendo la lógica de **Hechos (Ventas)** y **Dimensiones (Productos, Clientes, Tiempo)**.

---

## 🛠️ Flujo de Trabajo (Metodología)

El proyecto se dividió en etapas claras de transformación de datos:

### 1. ETL y Preparación de Datos
Se trabajó con dos datasets principales: `Master Global Super Store` (Transacciones) y `Products Global Super Store` (Maestro de Productos).
* **Limpieza:** Detección de valores nulos y estandarización de formatos de fecha y moneda.
* **Integración:** Uso de funciones de búsqueda (`VLOOKUP`/`INDEX-MATCH`) para cruzar los productos con las transacciones.
* **Modelado:** Creación de una tabla sábana ("Datos Procesados") que distingue entre métricas cuantitativas y dimensiones cualitativas.

### 2. Diseño y Prototipado (Mockup)
Antes de construir el dashboard final, se diseñó un prototipo para definir la distribución de la información y los KPIs necesarios.
> *Puedes ver el proceso de diseño en el archivo [`GUÍA DASHBOARD_MOCKUP_.pptx`](./GUÍA%20DASHBOARD_MOCKUP_.pptx)*.

### 3. Dashboard Interactivo
Se construyó un tablero de control dinámico en Google Sheets utilizando:
* **Tablas Dinámicas:** Para agregar grandes volúmenes de datos.
* **Slicers (Segmentadores):** Para permitir a la gerencia filtrar por año, región y categoría.
* **Gráficos Dinámicos:** Visualización de tendencias temporales y mapas geográficos.

---

## 📊 Visualización y Resultados

El resultado final permite una visión 360° de la operación.

| Mockup Inicial (Diseño) | Dashboard Final (Google Sheets) |
|:---:|:---:|
| ![Mockup](image_214698.png) | ![Dashboard Final](image_21465b.png) |
*(El dashboard permite filtrar por mercado, segmento y periodo)*

## 💡 Insights Clave y Hallazgos de Negocio

Tras el procesamiento y análisis de los datos (2013-2014), se presentaron las siguientes conclusiones estratégicas a la gerencia:

### 💰 Rentabilidad y Productos
* **Salud del Negocio:** La operación es altamente rentable, alcanzando un margen global cercano al **50%**.
* **La Joya de la Corona:** La categoría **"Office Supplies"** es la más eficiente con un **75% de rentabilidad**.
    * *Insight:* Aunque los "Binders" (Carpetas) generan el mayor volumen de ventas, son los **"Labels" (Etiquetas)** los que ofrecen el mayor margen de ganancia real.
* **Segmentación:** Si bien el "Consumidor Final" aporta el mayor volumen de ingresos, los segmentos corporativos ("Home Office" y "Corporate") son marginalmente más rentables, sugiriendo una oportunidad para estrategias B2B.

### 🌍 Análisis de Mercados (Geografía)
* **Volumen vs. Eficiencia:** Existe una clara distinción entre quién compra más y quién deja más dinero.
    * **Ingresos:** **APAC** (Asia-Pacífico) es el motor de ventas de la compañía ($34M+ en ventas).
    * **Rentabilidad:** **EMEA** (Europa, Oriente Medio y África) es la región más eficiente financiera, con una rentabilidad superior al **81%**.
* **Alerta en LATAM:** Latinoamérica se identificó como un punto crítico. Es el mercado menos rentable (**21.11%**) debido a una estructura de costos desproporcionadamente alta ($154M en costos vs $32M en ventas).
* **Oportunidades Ocultas:** El mercado africano y países específicos del EMEA (como Turquía y Eslovaquia) muestran rentabilidades superiores al 100%, señalando mercados ideales para expansión.

### 📦 Eficiencia Operativa y Logística
* **Método de Envío Óptimo:** "Standard Class" es el método dominante (más usado) y paradójicamente el más rentable (**59.11%**), superando ampliamente a los envíos "First Class" o "Same Day".
* **Ineficiencia en Prioridades:** Se detectó que los pedidos con **Prioridad Crítica** son los que **menor rentabilidad** generan.
    * *Recomendación:* Los pedidos de prioridad "Media" son los que sostienen los ingresos. Se recomienda auditar el proceso de asignación de urgencia, ya que los envíos críticos actuales están erosionando el margen de ganancia sin justificación financiera.

### 📅 Tendencias Temporales
* **Estacionalidad:** Se observa un patrón claro donde las ventas y la rentabilidad aumentan hacia el **segundo semestre del año** (Agosto-Diciembre), mientras que los primeros meses suelen presentar una baja en el volumen de negocio.

---

## 📁 Estructura del Repositorio

* `DATOS ORIGINALES.xlsx`: Datasets crudos provistos por la empresa.
* `DATOS PROCESADOS.xlsx`: Archivo principal con la limpieza de datos, tablas dinámicas y el **Dashboard Interactivo**.
* `GUÍA DASHBOARD_MOCKUP_.pptx`: Presentación con el diseño preliminar y la guía de usuario.
* `Informe.pdf`: Reporte ejecutivo con los hallazgos detallados.

---
**Autor:** Francisco Javier Hillebrand
[LinkedIn](Tu_Link_Aquí) | [Portafolio](Tu_Link_Aquí)
