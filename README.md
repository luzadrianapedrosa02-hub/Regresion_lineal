# Regresion_lineal
# Encuesta: Redes sociales y bienestar emocional

## Objetivo
Analizar cómo el uso de redes sociales influye en el bienestar emocional.

## Variable dependiente
- Nivel de bienestar emocional (0–10)

## Variables independientes
- Horas en redes sociales
- Edad
- Horas de sueño
- Frecuencia de ejercicio
- Tipo de contenido

## Encuesta
https://forms.office.com/Pages/ResponsePage.aspx?id=cZgrEyXgrU6jTXvV56ODtLIv-OtCdWRLrsPLJBzl8KhUMzhFUkowTFEyWDJWUjVYRERSVTdNOFdJRS4u

## Data Frame 
datos <- data.frame(
  Edad = c(24,27,25,23,19,26,25,23,24,25,24,30,24,26,26),
  Horas_Sueno = c(7,7,7,6,8,8,8,6,8,7,7,5,7,7,8),
  Horas_Redes = c(4,3,4,6,3,5,3,4,5,3,1,5,4,4,1),
  Ejercicio = c(4,4,2,3,6,1,3,4,1,2,4,1,3,5,4),
  Bienestar = c(7,7,3,7,9,8,8,8,6,7,9,1,5,7,9)
)

print(datos)

# Matriz Correlación 
cor(datos)

# Gráfica (bienestar vs horas en redes)
plot(datos$Horas_Redes, datos$Bienestar,
     main="Bienestar vs Uso de Redes Sociales",
     xlab="Horas en redes sociales",
     ylab="Bienestar (0-10)",
     col="blue",
     pch=19)

abline(lm(Bienestar ~ Horas_Redes, data=datos), col="red")

# Grafica (bienestar vs horas de sueño)
plot(datos$Horas_Sueno, datos$Bienestar,
     main="Bienestar vs Horas de sueño",
     xlab="Horas de sueño",
     ylab="Bienestar (0-10)",
     col="blue",
     pch=19)

abline(lm(Bienestar ~ Horas_Redes, data=datos), col="red")

# Regreción Lineal

modelo <- lm(Bienestar ~ Horas_Redes + Horas_Sueno + Ejercicio, data=datos)
summary(modelo)



