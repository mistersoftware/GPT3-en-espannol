# Indice de Contenidos

1. [Introducción](https://github.com/mistersoftware/GPT3-en-espannol/blob/master/01-Introduccion.md)
1. Enfoque
	1. Modelo y arquitecturas
	1. Datasets de entrenamiento
	1. Proceso de entrenamiento
	1. Evaluación
1. Resultados
	1. Modelado de lenguaje, Cloze y finalización de tareas
	1. Preguntas y respuestas a libro cerrado
	1. Traducción
	1. Tareas de Winograd-style
	1. Razonamiento de sentido común
	1. Comprensión lectora
	1. SuperGLUE
	1. NLI
	1. Tareas sintéticas y tareas cualitativas
1. Midiendo y preveniniendo la memorización de _benchmarks_
1. Limitaciones
1. Gran impacto
	1. Uso indebido de modelos de lenguaje
	2. Justicia, parcialidad (sesgo) y representación
	3. Uso de energía
1. Trabajo relacionado
1. Conclusión

# Resumen

## Trabajos recientes han demostrado grandes avances en tareas de procesamiento de lenguaje natural (PLN ó NLP en inglés) y en muchas comparativas (_benchmarks_) y  mediante el pre-entrenamiento sobre un gran corpus de texto, seguido de _fine-tuning_ sobre una tarea específica. 

[![](https://user-images.githubusercontent.com/12854504/88528064-be823c80-cfc3-11ea-8e5f-efef5b2c488e.gif)](https://platzi.com/comunidad/esto-me-trasnocha-la-consola-semantica/)


> Si bien la arquitectura es agnostica o independiente de la tarea, este método aún requiere _[fine-tuning](#)_ sobre _datasets_ de miles o decenas de miles de ejemplos. En contraste, los humanos pueden realizar una tarea nueva de lenguaje a partir de solo algunos ejemplos o instrucciones simples, -- _algo que los sistemas de PNL actuales todavía tienen muchas dificultades para hacer_ --. Aquí mostramos que al _escalar_ el tamaño del modelo se obtiene una gran mejora en el rendimiento en la modalidad de pocos intentos (_few shots_), a veces alcanzando incluso niveles de competitividad con enfoques anteriores de vanguardia. Específicamente, entrenamos GPT-3, un modelo de lenguaje autoregresivo (_transformer_) con 175 mil millones de parámetros, 10 veces más que cualquier modelo anterior no disperso (_non-sparse_), y probamos su rendimiento en la configuración _few shots_. 


Para todas las tareas, se aplica [GPT-3](#) sin ajuste del gradiente o _fine tunning_ demostrando la interacción del texto con el modelo. GPT-3 alcanza un alto rendimiento en diferentes _datasets_ de NLP, incluyendo tareas de traducción, responder preguntas, así como varias tareas que requieren razonamiento sobre la marcha o adaptación de dominio, tales como descifrar palabras, usar una palabra nueva en una oración, o realizar aritmética de 3 dígitos. 

Al mismo tiempo, también identificamos algunos _datasets_ donde el aprendizaje de _few shots_ de GPT-3 todavía tiene dificultades, así como algunos _datasets_ donde GPT-3 enfrenta problemas metodológicos relacionados con el entrenamiento basado en corpora de la web [GPT3 envenena GPT3](https://www.youtube.com/watch?v=VJ2mIFLxVTk). 

Finalmente, encontramos que GPT-3 puede generar muestras de [artículos de noticias](https://www.theverge.com/2020/5/30/21275524/microsoft-news-msn-layoffs-artificial-intelligence-ai-replacements) dificiles de distinguir por evaluadores humanos. Discutimos ademas los impactos sociales más amplios de este hallazgo y de GPT-3 en general.





