# David Fernando Valle Acosta | Data Scientist & ML Engineer 🤖

Físico por la UNAM y Científico de Datos especializado en el diseño de **pipelines robustos de Machine Learning (End-to-End)** y la optimización de infraestructuras de datos. Combino el rigor analítico de las ciencias exactas con estándares de ingeniería de software para transformar ecosistemas de datos masivos en modelos predictivos escalables y servicios web con alto valor de negocio.

### 🛠️ Arquitectura y Stack Tecnológico
* **Core ML & Modelado:** Python (Scikit-Learn, LightGBM, Pandas, NumPy, SciPy, SHAP).
* **Ingeniería de Datos & Optimización:** SQL, Apache Parquet (PyArrow), Joblib, Web Scraping (BS4).
* **Despliegue & Herramientas:** Render, Streamlit Cloud, GitHub Pages, Git/GitHub, VS Code, LaTeX.
* **Especialidades:** Aprendizaje Sensible al Costo (Cost-Sensitive), Evaluación de *Trade-offs*, Feature Engineering, Validación Temporal, Simulación Estocástica.

<p align="left">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white&color=9400D3" alt="Python"/>
  <img src="https://img.shields.io/badge/SQL-CC2927?style=for-the-badge&logo=postgresql&logoColor=white&color=FF00FF" alt="SQL"/>
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white&color=150458" alt="Pandas"/>
  <img src="https://img.shields.io/badge/Scikit--Learn-3499CD?style=for-the-badge&logo=scikit-learn&logoColor=white&color=2E64FE" alt="Scikit-Learn"/>
  <img src="https://img.shields.io/badge/LightGBM-F37021?style=for-the-badge&logo=databricks&logoColor=white&color=F37021" alt="LightGBM"/>
  <img src="https://img.shields.io/badge/Apache_Parquet-E2A446?style=for-the-badge&logo=apache&logoColor=white&color=298F43" alt="Apache Parquet"/>
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white&color=FF4500" alt="Streamlit"/>
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white&color=C70202" alt="Git"/>
</p>

---

### ⚙️ Proyectos Destacados

#### ⚡ [ERCOT Load Forecasting System: MLOps y Predicción Energética](https://github.com/DavidVaAc/ercot-load-forecasting)
Pipeline completo de MLOps de alta disponibilidad y modelo autoregresivo-termodinámico para el pronóstico de demanda por hora en la red eléctrica aislada de Texas.

* **Arquitectura de Failover en Cascada:** 

  Diseñé un backend redundante de 3 niveles para la extracción climática en tiempo real (Open-Meteo API ➔ Visual Crossing API ➔ Caché Local) asegurando un SLA continuo frente a interrupciones de servicios externos.

* **Rigor Metodológico y Validación Temporal:** 

  Entrené el LightGBM con bloques de datos de 2022-2024 y lo evalué ante un **año completo de prueba ciego (2025)**, logrando un extraordinario **MAPE base de 3.11%** tras modelar la respuesta no lineal (curva parabólica en U) del consumo energético.

* **Monitoreo de Degradación (*Model Decay*):** 

  Implementé un monitor dinámico en vivo dentro del servicio de **Streamlit Cloud** que calcula desviaciones del error contra la línea base de R&D, disparando alertas en semáforo (Verde/Naranja/Rojo) para notificar al operador sobre la necesidad de reentrenamiento.

#### 🏦 [Bank Churn Retention Framework: Cost-Sensitive Learning & MLOps](https://github.com/DavidVaAc/bank-churn-mlops-framework)
Ecosistema de producción automatizado y modular para la identificación, segmentación conductual y contención predictiva de la fuga de clientes en una cartera de tarjetas de crédito.

* **Motor Sensible al Costo (Cost-Sensitive Learning):** 

  Sustituí la optimización clásica de métricas puramente estadísticas (F1-Score/Accuracy) por un enfoque financiero basado en el valor de vida del cliente (LTV) y los costos operativos de alerta por clúster, maximizando el retorno de inversión (ROI) institucional.

* **Arquitectura de Inferencia Híbrida y Gobernanza:** 

  Diseñé un pipeline robusto desacoplado en 3 pilares (`main.py` para calibración asíncrona, `predict.py` para tareas batch CLI mensuales y `app.py` para simulación web) blindado por un split temporal de 3 vías (60/20/20) y un validador automatizado de contrato de datos (*input schema*).

* **Robustez de Clústeres y Simulación Estocástica:** 

  Implementé un remapeo determinista (Mapeo Canónico) para neutralizar la permutación arbitraria de etiquetas en K-Means, y un motor estocástico que ejecuta **10,000 simulaciones Monte Carlo (Bootstrap)** con un enfoque adaptativo de Valor Esperado Probabilístico para evaluar flujos financieros ante lotes de producción completamente ciegos.

* **Interpretabilidad y Despliegue Multi-Entorno:** 

  Entrené un clasificador LightGBM (**ROC-AUC de 0.9913**) auditado mediante valores **SHAP**, y desplegué un simulador estratégico interactivo en **Streamlit Cloud** que recalcula umbrales óptimos al vuelo e integra curvas de diagnóstico HTML dinámicas (Plotly) servidas nativamente en **GitHub Pages**.

#### 🛒 [Instacart Market Basket Analysis: Optimización y Analítica de Consumo](https://github.com/DavidVaAc/instacart-market-basket-analysis)
Extracción de inteligencia comercial y segmentación estratégica a partir de datos transaccionales masivos.

* **Ingeniería y Optimización:** 

  Procesé y depuré un ecosistema con más de **4.5 millones de registros**, implementando *downcasting* de tipos de datos para reducir drásticamente el consumo de memoria RAM.

* **Segmentación Estratégica (Pareto):** 

  Diseñé un modelo por deciles de volumen, identificando una concentración extrema donde solo el **0.04% del catálogo (18 productos)** genera el **10% de las ventas**, permitiendo priorizar la cadena de suministro.

* **Despliegue:** 
  
  Analicé dinámicas temporales de recompra y publiqué un dashboard interactivo en **Streamlit Cloud** con visualizaciones dinámicas en **Plotly**.

#### 🚗 [Car Price Regressor: Valuación Automatizada de Vehículos Usados](https://github.com/DavidVaAc/car-price-regressor)
Pipeline completo de Machine Learning y aplicación interactiva diseñada para automatizar la tasación comercial de vehículos de segunda mano.

* **Análisis de *Trade-off* en Producción:** 

  Evalué **6 algoritmos de regresión** no solo bajo métricas estadísticas de precisión, sino bajo criterios reales de ingeniería: **latencia de predicción y coste computacional**, seleccionando LightGBM como modelo final.

* **Garantía de Integridad (Frontend):** 

  Diseñé una interfaz con **filtros dinámicos en cascada** que mitiga el riesgo de "datos basura", asegurando que el modelo solo reciba combinaciones mecánicamente realistas.

* **Optimización de Infraestructura:** 

  Implementé almacenamiento en formato **Apache Parquet**, acelerando el tiempo de respuesta del servicio web y reduciendo el peso de lectura de los datos.

---

### 📫 Conectemos

* 💼 **Portafolio Interactivo:** [davidvaac.github.io/DavidVaAc](https://davidvaac.github.io/DavidVaAc/#)
* 🌐 **LinkedIn:** [in/david-fernando-valle-acosta](https://linkedin.com/in/david-fernando-valle-acosta)
* 📋 **Currículum Vitae:** [Descargar CV en PDF](https://drive.google.com/file/d/1qiQUyAmt3KGcFhBQ88-LPGflgPpHGs1m/view?usp=sharing)
* ✉️ **Email:** davidfervalle@gmail.com
* 📍 **Ubicación:** Cuernavaca, México.