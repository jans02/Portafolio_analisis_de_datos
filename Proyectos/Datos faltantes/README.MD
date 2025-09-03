# 📊 Datos Faltantes

## Contexto del Problema
En análisis de datos es común encontrar **valores faltantes (missing values)**.  

Estos pueden aparecer por diversas razones:

- ❌ Errores de captura de información.
- 🕒 Retrasos en la actualización de sistemas.
- 🔍 Datos no aplicables o no registrados.
- 📋 Limitaciones en encuestas o mediciones.  

La **presencia de datos faltantes** afecta la calidad del análisis, puede distorsionar modelos predictivos y comprometer la validez de los resultados. Por ello, es clave entender **su origen, impacto y tratamiento adecuado**.

Es por esto que se realiza este ejemplo, para comprender e identificar lo que pueden generar los datos faltantes.

---

## 🎯 Objetivo del Análisis
Evaluar la gestión de los **datos faltantes** considerando:

- 📊 Identificar la proporción de valores ausentes en el dataset.
- 📈 Analizar su impacto en métricas descriptivas y modelos predictivos.
- 🔍 Revisar métodos de imputación estadística (media, mediana, moda).
- 🤖 Explorar técnicas avanzadas basadas en algoritmos predictivos (ej. KNN).

Dicho análisis se realiza en la modificación de una data completa, a la cual se le elimina ciertos datos para poder lograr el objetivo

Este procedimiento se puede encontrar [aquí](https://colab.research.google.com/drive/1hSh3hYJDZ3gYiVDcU23w-LVVN-oMBv6i?usp=sharing)

---

## 💡 Hallazgos Clave
- **Incidencia de datos faltantes**: dependiendo del dataset, puede superar el **5%**, considerado crítico para modelado predictivo.  
- **Impacto en la media**: los valores faltantes reducen la representatividad y sesgan distribuciones.  
- **Impacto en la mediana**: más robusta que la media frente a valores atípicos, pero puede perder sensibilidad.  
- **Impacto en la moda**: útil en variables categóricas, aunque puede sobre-representar clases dominantes.  
- **Métodos avanzados**: técnicas como **KNN Imputer** aprovechan la información de otras variables para estimar los valores ausentes, mejorando precisión en datasets grandes.  

---

## 📌 Métodos de Tratamiento

| Método                  | Tipo de variable      | Ventajas                          | Limitaciones |
|--------------------------|----------------------|-----------------------------------|--------------|
| Eliminación de registros | Numéricas / Categ.   | Sencillo, evita sesgos artificiales | Pierde información valiosa |
| Media / Mediana / Moda   | Numéricas / Categ.   | Fácil implementación              | Distorsiona distribución si hay muchos faltantes |
| Imputación KNN           | Numéricas / Mixtas   | Considera similitud entre casos   | Computacionalmente costoso |

---

## 📋 Conclusiones
✅ Los **datos faltantes** son inevitables y deben tratarse de forma estratégica.  
✅ **Imputar con medidas de tendencia central** es adecuado para casos simples, pero puede introducir sesgos.  
✅ Existen **Métodos predictivos** (KNN, regresión, ML) más robustos, sin emvargo exigen mayor costo computacional.  
✅ La **elección del método** depende del porcentaje de datos ausentes, el tipo de variable y el objetivo del análisis.  

---

## 🔑 Recomendaciones
- 🚀 Aplicar imputación predictiva cuando los datos faltantes superen el **5%** del total.  
- 📉 Evitar eliminar registros salvo en casos donde los faltantes sean mínimos (<1%).  
- ⚙️ Usar **media/mediana/moda** solo cuando los datos ausentes sean bajos y aleatorios.  
- 🧩 Implementar **KNN Imputer** o técnicas de regresión en proyectos de machine learning.  
- 📊 Documentar siempre el proceso de imputación para mantener la trazabilidad del análisis. 
