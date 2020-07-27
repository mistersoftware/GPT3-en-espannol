## Trabajos recientes han demostrado grandes avances en tareas de procesamiento de lenguaje natural (PLN ó NLP en inglés) y en muchos comparativas (_benchmarks_) y  mediante el pre-entrenamiento sobre un gran corpus de texto seguido de un ajuste más preciso sobre una tarea específica. 

Si bien la arquitectura es agnostica o independiente de la tarea, este método aún requiere _[fine-tuning](#)_ sobre _datasets_ de miles o decenas de miles de ejemplos. En contraste, los humanos pueden realizar una tarea nueva de lenguaje a partir de solo algunos ejemplos o instrucciones simples, -- _algo que los sistemas de PNL actuales todavía tienen muchas dificultades para hacer_ --. 

> Aquí mostramos que al _escalar_ el tamaño del modelo se obtiene una gran mejora en el rendimiento en la modalidad de pocos intentos (_few shots_), a veces alcanzando incluso niveles de competitividad con enfoques anteriores de vanguardia. Específicamente, entrenamos GPT-3, un modelo de lenguaje autoregresivo (_transformer_) con 175 mil millones de parámetros, 10 veces más que cualquier modelo anterior no disperso (_non-sparse_), y probamos su rendimiento en la configuración _few shots_. 


[![](https://static.platzi.com/media/user_upload/EdGTFTcUMAEqlXf-1ff13759-a314-4e29-8099-ec229a12723c.jpg)](https://platzi.com/comunidad/mckay-wrigley-chateando-con-openai-gpt-3/)


Para todas las tareas, se aplica [GPT-3](#) sin ajuste del gradiente o _fine tunning_ demostrando la interacción del texto con el modelo. GPT-3 alcanza un alto rendimiento en diferentes _datasets_ de NLP, incluyendo tareas de traducción, responder preguntas, así como varias tareas que requieren razonamiento sobre la marcha o adaptación de dominio, tales como descifrar palabras, usar una palabra nueva en una oración, o realizar aritmética de 3 dígitos. 

Al mismo tiempo, también identificamos algunos _datasets_ donde el aprendizaje de _few shots_ de GPT-3 todavía tiene dificultades, así como algunos _datasets_ donde GPT-3 enfrenta problemas metodológicos relacionados con el entrenamiento basado en corpora de la web [GPT3 envenena GPT3](https://www.youtube.com/watch?v=VJ2mIFLxVTk). 

Finalmente, encontramos que GPT-3 puede generar muestras de [artículos de noticias](https://www.theverge.com/2020/5/30/21275524/microsoft-news-msn-layoffs-artificial-intelligence-ai-replacements) dificiles de distinguir por evaluadores humanos. Discutimos ademas los impactos sociales más amplios de este hallazgo y de GPT-3 en general.


