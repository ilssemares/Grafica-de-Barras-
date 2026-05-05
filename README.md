# Grafica-de-Barras-
De acuerdo con el observatorio ciudadano este es el índice de las personas que confían en las instituciones 
<img width="1206" height="749" alt="image" src="https://github.com/user-attachments/assets/29e38bb2-6ad2-4e0d-bb92-f9df04a0785f" />
# CODIGO DE PROGRAMACION 

df_barras <- data.frame(
  institucion = c("Gobierno", "INE", "Policía", "Ejército", "Medios"),
  personas = c(25, 55, 30, 60, 35)
)


print(df_barras)


ggplot(df_barras, aes(x = institucion, y = personas))+
  geom_col(aes(fill = institucion))+
  labs(
    title = "Cantidad de personas que confian",
    x = "Institucion",
    y = "Número de personas"
  ) +
  theme_minimal()
