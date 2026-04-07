🌐 **Lenguaje:**  
[English version](README_EN.md)

# 📊 Análisis de Producto Prueba A/B

## 📌 Descripción
Este proyecto analiza el impacto de un cambio en las fuentes tipográficas de
una aplicación de una empresa alimenticia, utilizando un experimento A/A/B
para evaluar si la modificación genera un efecto significativo en el
comportamiento de los usuarios.

El análisis se centra en el comportamiento de los usuarios a lo largo de un
embudo de eventos, validando primero la equivalencia de los grupos de control
(A/A) y posteriormente evaluando el efecto del cambio tipográfico (A/B).

## 🧠 Objetivo
- Evaluar si un cambio de tipografía impacta el comportamiento del usuario
- Validar la correcta asignación de usuarios mediante un test A/A
- Analizar el embudo de eventos dentro de la aplicación
- Aplicar pruebas estadísticas con corrección por pruebas múltiples
- Emitir conclusiones basadas en evidencia estadística

## 📂 Estructura del proyecto
- `datasets/` → Dataset del experimento
- `notebooks/` → Análisis A/A/B en Jupyter Notebook
- `README.md` → Descripción del proyecto en español
- `README_EN.md` → Descripción del proyecto en inglés
- `requirements.txt` → Dependencias del proyecto

## 🔬 Metodología
- Limpieza y procesamiento de datos
- Análisis exploratorio del comportamiento de usuarios
- Construcción del embudo de eventos
- Test A/A para validar equivalencia entre grupos de control
- Test A/B para evaluar el impacto del cambio tipográfico
- Ajuste del nivel de significancia por pruebas múltiples

## 🛠️ Tecnologías utilizadas
- Python
- Pandas
- NumPy
- SciPy
- Matplotlib / Seaborn
- Jupyter Notebook

## 📈 Resultados

El objetivo principal del experimento fue evaluar si la modificación en las
fuentes tipográficas de la aplicación generaba un impacto significativo en el
comportamiento de los usuarios. Para ello, se implementó un experimento A/A/B
con dos grupos de control (246 y 247) y un grupo de prueba (248) expuesto al
nuevo diseño.

Los resultados del análisis permiten extraer las siguientes conclusiones:

- **Validez del experimento:**  
  La comparación entre los dos grupos de control no mostró diferencias
  estadísticamente significativas en ninguno de los eventos analizados,
  confirmando que la aleatorización fue exitosa y que el experimento está
  correctamente implementado.

- **Impacto del rediseño:**  
  Al comparar el grupo con la nueva tipografía (248) frente a los grupos de
  control, no se identificaron diferencias estadísticamente significativas en
  los eventos clave del embudo de conversión (pantalla principal, ofertas,
  carrito, pago y tutorial).

- **Robustez estadística:**  
  Se realizaron 15 pruebas de hipótesis y, tras aplicar la corrección de
  Bonferroni para controlar el riesgo de falsos positivos, todas las
  conclusiones se mantuvieron consistentes. El valor p más bajo observado
  permaneció por encima del umbral ajustado (0.0033), lo que indica ausencia
  de un efecto atribuible al rediseño.

En conclusión, dado que el cambio tipográfico no genera un impacto negativo en
el comportamiento de los usuarios, se recomienda su implementación completa.
Además, el experimento valida la solidez del sistema de experimentación del
producto y establece una base confiable para futuras pruebas A/B de mayor
complejidad.


