# Detección de Phishing mediante Machine Learning

Este repositorio contiene la investigación y el desarrollo técnico de mi Trabajo de Fin de Grado (TFG) para la titulación de Ingeniería Informática. El proyecto desarrolla un sistema de clasificación de URLs maliciosas utilizando un motor de extracción híbrido y comparando arquitecturas de aprendizaje supervisado.

## Estructura del Repositorio

* **notebooks/**: 
    * Estudio_de_obsolescencia.ipynb: Análisis del impacto temporal en los patrones de ataque (Datasets 2018 vs 2024).
    * Estudio_de_algoritmos.ipynb: Evaluación y optimización de modelos (Random Forest, SVM y XGBoost).
* **data/**:
    * **raw/**: Datasets originales. Nota: El dataset de 2024 se encuentra comprimido en `.zip` debido a las limitaciones de tamaño de GitHub.
    * **processed/**: Características extraídas. El archivo `vivas_phi_cache_FULL.zip` contiene el dataset de 2024 procesado con 234.000 muestras procedentes de PhiUSIIL, categorizadas según su estado (Online y Offline).

## Diccionario de Datos (Etiquetado)
El etiqutado usado en todos los datasets procesados fue el siguiente:
* **0**: Phishing 
* **1**: Legítimo 

## Citas y Fuentes de Datos
Este estudio se basa en los siguientes conjuntos de datos públicos:
1. **PhiUSIIL Phishing Dataset (https://doi.org/10.1016/j.cose.2023.103545)**: Dataset contemporáneo utilizado para el entrenamiento y modelado principal.
2. **Dataset 2018 (https://github.com/ebubekirbbr/pdd/tree/master/input)**: Conjunto de datos antiguo utilizado para el estudio de obsolescencia de patrones de ataque.
3. **PhishTank (https://www.phishtank.com)**: Muestras activas de 2026 obtenidas para la validación externa del sistema.

## Tecnologías Utilizadas
* **Lenguaje:** Python 3.10+
* **Librerías:** `scikit-learn`, `xgboost`, `pandas`, `numpy`, `matplotlib`, `seaborn`.

---
## Autor

Sergio Cano San José  
Grado en Ingeniería Informática  
Trabajo de Fin de Grado
