# Bienestar emocional y factores asociados

## Descripción del proyecto

Este proyecto analiza la relación entre el **bienestar emocional** y tres factores de estilo de vida:  
- uso de redes sociales  
- horas de sueño  
- actividad física (ejercicio)

El objetivo es identificar patrones de asociación entre estos factores y el nivel de bienestar mediante análisis estadístico exploratorio.

---

## Objetivo

Evaluar la relación entre hábitos de vida (redes sociales, sueño y ejercicio) y el bienestar emocional, utilizando análisis de correlación y regresión lineal.

---

## Variables del estudio

- **Bienestar:** escala de 0 a 10  
- **Horas de sueño:** promedio diario  
- **Horas en redes sociales:** uso diario  
- **Ejercicio:** actividad física semanal  

---

## Resultados

### 1. Matriz de correlación

Se aplicó correlación de Pearson para identificar relaciones lineales entre variables.

**Resultados generales:**
- Redes sociales → relación negativa con bienestar  
- Sueño → relación positiva con bienestar  
- Ejercicio → relación positiva con bienestar  

 *Figura 1: Matriz de correlación*  
<img width="860" height="517" alt="Rplot01" src="https://github.com/user-attachments/assets/e91b05b3-99d4-4b72-aeec-8fa36d925566" />
---

### 2. Análisis bivariado

Con el objetivo de profundizar en las relaciones observadas en la matriz de correlación, se realizaron gráficos de dispersión con ajuste lineal para cada variable explicativa respecto al bienestar.

#### Redes sociales vs bienestar  
Se observa una relación negativa fuerte entre el uso de redes sociales y el bienestar emocional. En términos del modelo lineal, cada hora adicional en redes sociales se asocia con una disminución aproximada de 1.18 puntos en el bienestar.

 *Figura 2: Redes sociales vs bienestar*  
<img width="860" height="517" alt="Rplot02" src="https://github.com/user-attachments/assets/a3edddc4-c048-4bfc-94b6-e67ca341b130" />
---

#### Sueño vs bienestar  
Se identifica una relación positiva fuerte entre las horas de sueño y el bienestar. Específicamente, una hora adicional de sueño se asocia con un incremento aproximado de 1.94 puntos en el bienestar.

Este es el efecto más fuerte observado en el análisis bivariado, lo que sugiere que el descanso es un factor clave en la explicación del bienestar emocional.

*Figura 3: Sueño vs bienestar*  
<img width="860" height="517" alt="Rplot03" src="https://github.com/user-attachments/assets/f95b5bb9-95b7-4236-8226-9794e7e94141" />
---

#### Ejercicio vs bienestar  
Se observa una relación positiva fuerte entre la actividad física y el bienestar. En promedio, un aumento en el nivel de ejercicio se asocia con un incremento de aproximadamente 1.14 puntos en el bienestar.

*Figura 4: Ejercicio vs bienestar*  
<img width="860" height="517" alt="Rplot04" src="https://github.com/user-attachments/assets/451f2105-98aa-44e0-9f82-3036e0bd9918" />
---

### 3. Modelo de regresión múltiple

Se aplicó un modelo de regresión lineal múltiple para analizar el efecto conjunto de las variables.

*Figura 5: Regresión Lineal*  
<img width="997" height="426" alt="2026-04-20" src="https://github.com/user-attachments/assets/1bb09387-1c3f-43d2-aa6f-6825bc698007" />
---

**Resultados clave:**
- El modelo explica parte de la variabilidad del bienestar.
- Sueño y ejercicio tienden a mostrar efectos positivos.
- Redes sociales tienden a mostrar un efecto negativo.
- El modelo permite evaluar el impacto simultáneo de los factores.



## 🧾 Conclusiones
Los resultados del modelo de regresión lineal múltiple muestran que los hábitos de vida tienen una relación significativa con el bienestar emocional. En particular, las horas de sueño y la actividad física presentan efectos positivos y estadísticamente significativos, lo que sugiere que ambos factores contribuyen de manera importante al bienestar.

Por otro lado, aunque el uso de redes sociales presenta un coeficiente negativo, este no resulta estadísticamente significativo al controlar por otras variables, lo que indica que su efecto podría estar mediado por factores como el sueño o el ejercicio.

El modelo presenta un buen nivel de ajuste (R² ≈ 0.78), lo que indica que una proporción considerable de la variabilidad del bienestar es explicada por las variables incluidas.

Sin embargo, dado el carácter exploratorio del análisis, los resultados deben interpretarse como asociaciones y no como relaciones causales.

## Autor
Luz Adriana Espinosa Pedroza


