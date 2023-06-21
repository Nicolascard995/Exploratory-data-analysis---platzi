# Exploratory-data-analysis---platzi
Curso de EDA. 


Cómo hacer un análisis exploratorio de datos?
En este repositorio, comparto un Jupyter Notebook que desarrollé durante mi curso de Análisis Exploratorio de Datos (EDA) en Platzi. El curso proporciona una comprensión profunda de cómo se pueden explorar, analizar y sintetizar grandes conjuntos de datos para extraer información valiosa y tomar decisiones informadas. Aquí hay un resumen de lo que aprenderás:

Organizar y entender las variables: Identificarás los diferentes tipos de variables, las categorías a las que pertenecen y el tipo de análisis que puedes realizar sobre ellas.
Establecer relaciones entre las variables
Encontrar patrones ocultos en los datos: Encontrarás información o comportamientos relevantes cuando hagas el EDA.
Ayuda a escoger el modelo correcto para la necesidad correcta: Una vez encuentres cómo están relacionadas las variables, podrás descubrir las variables que más se ajustan a un tipo de modelo y de esta manera elegirás el correcto.
Ayuda a tomar decisiones informadas: Decisiones basadas en los datos, en las relaciones que encuentres entre variables, en patrones ocultos y en los modelos que generes a través de la EDA.
Pasos de un Análisis Exploratorio de Datos
Hacer preguntas sobre los datos. Hazte las siguientes preguntas para guiar el EDA:
¿Qué te gustaría encontrar?
¿Qué quisieras saber de los datos?
¿Cuál es la razón para realizar el análisis?
Determinar el tamaño de los datos. Debes responder preguntas como:
¿Cuántas observaciones existen?
¿Cuántas variables hay?
¿Necesito todas las observaciones?
¿Necesito todas las variables?
Categorizar las variables. Debes preguntarte:
¿Cuántas variables categóricas existen?
¿Cuántas variables continuas existen?
¿Cómo puedo explorar cada variable dependiendo de su categoría?
Limpieza y validación de los datos. En este paso debes preguntarte:
¿Tengo valores faltantes?
¿Cuál es la proporción de datos faltantes?
¿Cómo puedo tratar a los datos faltantes?
¿Cuál es la distribución de los datos?
¿Tengo valores atípicos?
Establecer relaciones entre los datos. Responde preguntas como:
¿Existe algún tipo de relación entre mi variable X y Y?
¿Qué pasa ahora si considero la variable Z en el análisis?
¿Qué significa que las observaciones se agrupen?
¿Qué significa el patrón que se observa?
Entorno de desarrollo: Deepnote
Realicé este proyecto en Deepnote, una plataforma de desarrollo de Jupyter Notebook en la nube. Deepnote ofrece varias ventajas para los científicos de datos:

Acceso en cualquier lugar: Como plataforma basada en la nube, puedes acceder a tus notebooks desde cualquier lugar con una conexión a internet.
Colaboración en tiempo real: Deepnote permite la colaboración en tiempo real, similar a Google Docs. Esto es especialmente útil para los proyectos en equipo.
Integracióncon GitHub: Puedes sincronizar tus notebooks con tus repositorios de GitHub, lo que facilita el seguimiento de versiones y la colaboración.
Recursos informáticos escalables: Deepnote te permite ajustar los recursos informáticos según tus necesidades, lo que es útil para trabajar con grandes conjuntos de datos o realizar cálculos intensivos.
Entorno completamente administrado: No tienes que preocuparte por la configuración del entorno o la gestión de dependencias, ya que Deepnote se encarga de todo eso por ti.
Código
Para comenzar, asegúrate de tener todas las bibliotecas necesarias instaladas. Puedes hacerlo ejecutando los siguientes comandos en tu notebook:

python
Copy code
!pip install --upgrade pip
python
Copy code
!pip install palmerpenguins==0.1.4 numpy==1.23.4 pandas==1.5.1 seaborn==0.12.1 matplotlib==3.6.0 empiricaldist==0.6.7 statsmodels==0.13.5 scikit-learn==1.1.2 pyjanitor==0.23.1 session-info
A continuación, importa todas las bibliotecas necesarias para el análisis:

python
Copy code
import empiricaldist
import janitor
import matplotlib.pyplot as plt
import numpy as np
import palmerpenguins
import pandas as pd
import scipy.stats
import seaborn as sns
import sklearn.metrics
import statsmodels.api as sm
import statsmodels.formula.api as smf
import statsmodels.stats as ss
import session_info

%matplotlib inline
sns.set_style(style='whitegrid')
sns.set_context(context='notebook')
plt.rcParams['figure.figsize'] = (11, 9.4)

penguin_color = {
    'Adelie': '#ff6602ff',
    'Gentoo': '#0f7175ff',
    'Chinstrap': '#c65dc9ff'
}
¡Ahora estás listo para comenzar tu análisis exploratorio de datos!
