# 📊 Análisis Exploratorio de Datos (EDA) – Exportaciones de Chile

---

## 📝 Contexto del Problema
El análisis de exportaciones es clave para entender el flujo comercial de Chile hacia diferentes países.  

Mediante un **EDA (Exploratory Data Analysis)** se pueden detectar patrones, identificar mercados clave, analizar productos estratégicos y evaluar la contribución regional.  

Durante el proceso también se revisa la **calidad de los datos**, como valores faltantes o atípicos, ya que pueden distorsionar el análisis y afectar la toma de decisiones.

El análisis principal se encuentra en el siguiente collab

---

## 🎯 Objetivo del Análisis
- 📊 Explorar las exportaciones de Chile clasificadas por **producto, región de origen y país de destino**.  
- 🔍 Identificar **países destino principales** y su peso económico.  
- 🍇 Detectar los **productos más relevantes** en volumen y valor exportado.  
- 🌎 Analizar la **participación de regiones** en las exportaciones.  
- 📈 Visualizar **patrones multivariados** con gráficos comparativos (barras, heatmaps, burbujas).  

---

## 💡 Hallazgos Clave

### 🔎 Calidad de datos
- No se detectaron **valores faltantes** en el dataset.  
- Se identificaron **valores atípicos** en `Volumen` (≈ 5.843) y en `USD FOB` (≈ 4.705), los cuales fueron tratados con imputación por mediana.  

### 📊 Análisis univariado
- **Volumen**: distribuciones sesgadas, con algunos valores extremos.  
- **USD FOB**: rango amplio con casos negativos que se trataron como errores o outliers.  
- **Categorías**:
  - Unidad más frecuente: **Kilo neto**.  
  - Productos dominantes: **vinos** y **frutas frescas**.  
  - Regiones líderes: **Metropolitana, O’Higgins y Maule**.  

### 🌎 Análisis multivariado
- **Top 10 países destino** concentran la mayoría de exportaciones, destacando EE.UU., China y Japón.  
- **Heatmap Producto–País** evidencia que vinos y frutas se concentran en mercados específicos.  
- **Gráfico de burbujas** muestra relaciones:  
  - Eje X: País destino.  
  - Eje Y: Producto.  
  - Tamaño: Volumen exportado.  
  - Color: USD FOB.  
  → Claramente se concentran envíos de alto valor en pocos productos-países.  

---

## 📋 Conclusiones
✅ Chile depende fuertemente de **pocos mercados y productos**, lo que genera vulnerabilidad ante cambios de demanda o políticas comerciales.  
✅ Algunas **regiones concentran la mayoría de exportaciones**, lo cual refleja disparidades territoriales.  
✅ El tratamiento de **outliers e imputación** mejora la consistencia de las métricas descriptivas.  
✅ Los gráficos multivariados permiten **detectar nichos de diversificación** y posibles oportunidades de expansión.  

---

## 🔑 Recomendaciones
- 🚀 **Diversificar mercados**: reducir la dependencia de unos pocos países compradores.  
- 🍇 **Promover nuevos productos exportables**, más allá de los vinos y frutas frescas.  
- 🗺️ **Fortalecer regiones con baja participación** para equilibrar el desarrollo territorial.  
- 📉 **Monitorear outliers y calidad de datos** en futuras cargas de información.  
- 🤖 En modelos predictivos, usar técnicas robustas como **KNN Imputer** o regresión para mejorar la precisión frente a valores faltantes o atípicos.  

