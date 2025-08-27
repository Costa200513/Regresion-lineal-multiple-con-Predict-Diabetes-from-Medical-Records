# Predicción de Diabetes con Regresión Lineal Múltiple

## Introducción
Este proyecto utiliza un **modelo de regresión lineal múltiple** para estimar la probabilidad de que un paciente tenga diabetes. El modelo se entrena con variables clínicas seleccionadas del dataset *Predict Diabetes from Medical Records*: **Glucosa, IMC y Edad**. La idea es poder predecir riesgos a partir de valores médicos y comprender qué factores influyen más en la probabilidad de desarrollar diabetes.

## Justificación de la elección de variables
- **Glucosa:** Es el indicador más directo de diabetes; niveles altos aumentan significativamente el riesgo.  
- **IMC:** Un IMC elevado indica sobrepeso u obesidad, factores que contribuyen a la resistencia a la insulina.  
- **Edad:** El riesgo de diabetes aumenta con la edad, siendo un factor no modificable pero importante para la predicción.  

Estas variables permiten construir un modelo simple, interpretable y con sentido médico, equilibrando precisión y facilidad de uso.

## Casos de prueba

### 1. Joven con diabetes
- **Edad:** 25 años  
- **Glucosa:** 170 mg/dL  
- **IMC:** 35  
**Probabilidad estimada:** 63 %  
> A pesar de la juventud, los valores altos de glucosa y IMC aumentan significativamente el riesgo.

### 2. Viejo con diabetes
- **Edad:** 65 años  
- **Glucosa:** 160 mg/dL  
- **IMC:** 30  
**Probabilidad estimada:** 72 %  
> La combinación de edad avanzada, glucosa elevada y sobrepeso genera la probabilidad más alta entre los casos.

### 3. Viejo sin diabetes
- **Edad:** 70 años  
- **Glucosa:** 95 mg/dL  
- **IMC:** 24  
**Probabilidad estimada:** 29 %  
> Valores normales de glucosa e IMC reducen significativamente el riesgo, incluso con edad avanzada.

### 4. Joven sin diabetes
- **Edad:** 22 años  
- **Glucosa:** 90 mg/dL  
- **IMC:** 25  
**Probabilidad estimada:** 3 %  
> La juventud combinada con parámetros normales de glucosa e IMC mantiene la probabilidad muy baja.

## Conclusión
El modelo confirma que **la glucosa es el factor más determinante**, seguido de IMC y edad.  
- Pacientes jóvenes con glucosa o IMC elevados pueden tener un riesgo considerable.  
- La edad aumenta el riesgo cuando se combina con valores clínicos desfavorables.  
- Mantener glucosa e IMC dentro de rangos normales reduce la probabilidad de diabetes, independientemente de la edad.  

Este análisis permite comprender cómo las variables clínicas influyen en la predicción y ofrece un ejemplo práctico de uso de regresión lineal múltiple para estimar riesgos médicos.
