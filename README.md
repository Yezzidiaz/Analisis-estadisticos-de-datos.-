# 📊 Análisis Estadísticos de Datos — Megaline  

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-blue?logo=python" />
  <img src="https://img.shields.io/badge/Pandas-Limpieza%20de%20Datos-150458?logo=pandas" />
  <img src="https://img.shields.io/badge/NumPy-Cálculos%20Vectoriales-orange?logo=numpy" />
  <img src="https://img.shields.io/badge/Matplotlib-Visualización-11557c?logo=plotly" />
  <img src="https://img.shields.io/badge/SciPy-Pruebas%20Estadísticas-8CAAE6?logo=scipy" />
  <img src="https://img.shields.io/badge/Status-Proyecto%20Académico-success" />
</p>

---

## 📌 Descripción del proyecto

Este proyecto analiza los datos de **500 clientes de Megaline**, un operador de telecomunicaciones con dos tarifas prepago:

- 🟦 **Surf**
- 🟩 **Ultimate**

El objetivo es determinar **cuál de las dos tarifas genera más ingresos** para mejorar la estrategia comercial y optimizar campañas publicitarias.

Para ello se estudian:

- Uso de **llamadas**
- Envío de **mensajes**
- Consumo de **Internet**
- **Ingresos mensuales** generados por cada usuario
- Diferencias de comportamiento entre planes
- Comparaciones por **región geográfica**

## 🧰 Herramientas utilizadas

-🐍 **Python 3.x**  
-📚 **Pandas**, **NumPy**  
-📊 **Matplotlib**, **Seaborn**  
-🧪 **SciPy (stats)**  
-📝 Archivos CSV: llamadas, internet, mensajes, planes y usuarios  

## 🗂️ Datos del proyecto

Los datasets incluyen:

- `users.csv` — datos demográficos, plan, registro y churn  
- `plans.csv` — condiciones de cada plan (minutos, SMS, GB, precios)  
- `calls.csv` — duración y fecha de cada llamada  
- `messages.csv` — fecha de cada SMS  
- `internet.csv` — tráfico por sesión (MB usados)  

## 🎯 Acciones principales del análisis

### 🔧 1. Preparación y limpieza
- Conversión de fechas  
- Eliminación de duplicados  
- Tratamiento de duraciones 0 o negativas  
- Conversión MB → GB  
- Unión de tarifas con usuarios  
- Agrupación mensual por usuario  

### 📊 2. Análisis del comportamiento del usuario

#### 📞 Llamadas
- Usuarios de **Ultimate** realizan más minutos mensuales.  
- La variabilidad del consumo es mayor en Ultimate.

#### ✉️ Mensajes
- Ultimate manda más mensajes en promedio.  
- Surf muestra un patrón más estable y bajo.

#### 🌐 Internet
- Ultimate consume más GB promedio.  
- Ambos planes tienen dispersión similar, con uso más alto en Ultimate.

### 💰 3. Análisis de ingresos

- **Ultimate genera más ingresos promedio mensuales** que Surf.  
- Se detecta un ingreso mayor en regiones como **NY–NJ**.

### 🧪 4. Pruebas estadísticas aplicadas

#### 1️⃣ Surf vs Ultimate (ingresos)
- **H₀:** ingresos promedio iguales  
- **Resultado:** ❌ Se rechaza — hay diferencia significativa  
- Ultimate es más rentable.

#### 2️⃣ NY–NJ vs otras regiones
- **H₀:** ingresos promedio iguales  
- **Resultado:** ❌ Se rechaza — NY–NJ consume más y genera mayores ingresos.

## 🧾 Conclusiones principales

✔️ Los usuarios de **Ultimate** consumen más minutos, GB y mensajes.  
✔️ **Ultimate genera más ingresos**, de forma estadísticamente significativa.  
✔️ La región **NY–NJ** muestra un comportamiento de consumo más alto.  
✔️ Surf es usado principalmente por usuarios de bajo consumo.  

📌 **Recomendación**:  
Aumentar inversión publicitaria en Ultimate y en regiones de alto consumo como NY–NJ, optimizando campañas segmentadas.

