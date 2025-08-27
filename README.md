# Predicción de Diabetes con Regresión Lineal Múltiple

---

## Introducción
Este proyecto utiliza un **modelo de regresión lineal múltiple** para estimar la probabilidad de que un paciente tenga diabetes.  
El modelo se entrena con variables clínicas seleccionadas del dataset *Predict Diabetes from Medical Records*: **Glucosa, IMC y Edad**.  
El objetivo es predecir riesgos a partir de valores médicos y comprender qué factores influyen más en la probabilidad de desarrollar diabetes.

---

## Justificación de la elección de variables
- **Glucosa:** Es el indicador más directo de diabetes; niveles altos aumentan significativamente el riesgo.  
- **IMC:** Un IMC elevado indica sobrepeso u obesidad, factores que contribuyen a la resistencia a la insulina.  
- **Edad:** El riesgo de diabetes aumenta con la edad, siendo un factor no modificable pero importante para la predicción.  

Estas variables permiten construir un modelo simple, interpretable y con sentido médico, equilibrando precisión y facilidad de uso.

---

## Casos de prueba

### 1️⃣ Joven con diabetes
- **Glucosa:** 170 mg/dL  
- **IMC:** 35  
- **Edad:** 25 años  
- **Probabilidad estimada:** 63 %  

<img width="577" height="252" alt="image" src="https://github.com/user-attachments/assets/6048df56-63ca-4738-a538-1b4645e71676" />

> A pesar de la juventud, los valores altos de glucosa y IMC aumentan significativamente el riesgo.

---

### 2️⃣ Viejo con diabetes
- **Glucosa:** 160 mg/dL  
- **IMC:** 30  
- **Edad:** 65 años  
- **Probabilidad estimada:** 72 %  

<img width="578" height="256" alt="image" src="https://github.com/user-attachments/assets/dcd71057-128c-48fa-8aa0-7264dfcc3b18" />

> La combinación de glucosa elevada, IMC alto y edad avanzada genera la probabilidad más alta entre los casos.

---

### 3️⃣ Viejo sin diabetes
- **Glucosa:** 95 mg/dL  
- **IMC:** 24  
- **Edad:** 70 años  
- **Probabilidad estimada:** 29 %  

<img width="587" height="259" alt="image" src="https://github.com/user-attachments/assets/22d66e26-ae60-44a5-ac15-d442695e7dbf" />

> Valores normales de glucosa e IMC reducen significativamente el riesgo, incluso con edad avanzada.

---

### 4️⃣ Joven sin diabetes
- **Glucosa:** 90 mg/dL  
- **IMC:** 25  
- **Edad:** 22 años  
- **Probabilidad estimada:** 3 %  

<img width="581" height="256" alt="image" src="https://github.com/user-attachments/assets/395f3f08-f61e-49c2-b953-3271020f51b2" />

> La juventud combinada con parámetros normales de glucosa e IMC mantiene la probabilidad muy baja.

---

## Conclusión
El modelo confirma que **la glucosa es el factor más determinante**, seguido de IMC y edad.  

- Pacientes jóvenes con glucosa o IMC elevados pueden tener un riesgo considerable.  
- La edad aumenta el riesgo cuando se combina con valores clínicos desfavorables.  
- Mantener glucosa e IMC dentro de rangos normales reduce la probabilidad de diabetes, independientemente de la edad.  

Este análisis permite comprender cómo las variables clínicas influyen en la predicción y ofrece un ejemplo práctico de uso de regresión lineal múltiple para estimar riesgos médicos.

---
