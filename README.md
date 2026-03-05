# Challenge-Telecon-X2-Jonatan-Alexander-Bejarano-Avila
# 📊 Análisis de Churn — TelecomX

Análisis exploratorio y modelado predictivo de la cancelación de clientes (churn) en una empresa de telecomunicaciones, utilizando Python y Machine Learning.

## 🎯 Objetivo

Identificar los **factores clave** que llevan a los clientes a cancelar su servicio y construir un modelo predictivo que permita detectar clientes en riesgo de churn para activar campañas de retención proactivas.

## 📁 Estructura del Proyecto

| Archivo | Descripción |
|---|---|
| [telecomx_parte2.ipynb](cci:7://file:///c:/Users/jonat/OneDrive/Desktop/reloj/telecomx_parte2.ipynb:0:0-0:0) | Notebook principal con el análisis completo (EDA, visualizaciones y modelado) |
| [datos_tratados.csv](cci:7://file:///c:/Users/jonat/OneDrive/Desktop/reloj/datos_tratados.csv:0:0-0:0) | Dataset limpio con 7,043 clientes y 21 variables |

## 🛠️ Tecnologías Utilizadas

- **Python 3**
- **Pandas** — Manipulación y análisis de datos
- **NumPy** — Operaciones numéricas
- **Matplotlib & Seaborn** — Visualización de datos
- **Scikit-learn** — Modelos de Machine Learning

## 📈 Metodología

1. **Carga y limpieza de datos** — Tratamiento de valores nulos y variables redundantes
2. **Análisis exploratorio (EDA)** — Distribuciones, correlaciones y pruebas Chi-Cuadrado
3. **Selección de variables** — Eliminación de variables sin relevancia estadística (`Gender`, `PhoneService`, cargos redundantes)
4. **Modelado predictivo** — Entrenamiento y evaluación de:
   - Regresión Logística
   - Random Forest
   - Regresión Logística Balanceada

## 🔑 Hallazgos Principales

- El **tipo de contrato** es el factor más determinante: contratos mensuales tienen **42.7% de churn** vs 2.8% en contratos de dos años
- Clientes **sin seguridad online** ni **soporte técnico** tienen el doble de probabilidad de cancelar
- El pago por **cheque electrónico** presenta el churn más alto: **45.3%**
- **Adultos mayores** sin dependientes son un grupo de alto riesgo (41.7% churn)

## 🏆 Mejor Modelo

| Modelo | Accuracy | Recall (Churn) | F1 (Churn) |
|---|---|---|---|
| Reg. Logística Balanceada | 74% | **79%** | **0.62** |

> La **Regresión Logística Balanceada** es el modelo más útil para el negocio: detecta el **79%** de los clientes que van a cancelar, priorizando la retención sobre la precisión.

## 💡 Recomendaciones Estratégicas

1. Migrar contratos mensuales a anuales con incentivos
2. Investigar los problemas con el cobro por cheque electrónico
3. Ofrecer paquetes de seguridad online + soporte técnico
4. Crear programas de atención especial para adultos mayores
5. Implementar alertas tempranas con el modelo balanceado
6. Revisar la calidad del servicio de fibra óptica

## 🚀 Cómo Ejecutar

1. Clona el repositorio:
   ```bash
   git clone https://github.com/tu-usuario/telecomx-churn-analysis.git
