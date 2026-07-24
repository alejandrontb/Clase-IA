# Actividad de Clase: Analizando Agentes de IA con Hugging Face Spaces

## Objetivo

Explorar aplicaciones reales de Inteligencia Artificial en **Hugging
Face Spaces** y analizarlas desde la perspectiva de los **agentes
racionales**.

Al finalizar la actividad, los estudiantes deberán ser capaces de:

-   Identificar los componentes **PEAS** de un agente.
-   Clasificar las propiedades del entorno.
-   Proponer qué tipo de programa de agente podría implementarse detrás
    del sistema.
-   Justificar sus respuestas.

------------------------------------------------------------------------

## Instrucciones

1.  Ingresen a **https://huggingface.co/spaces**.
2.  Exploren diferentes Spaces.
3.  Seleccionen uno que les parezca interesante.
4.  Interactúen con el sistema durante algunos minutos.
5.  Completen la siguiente ficha de análisis.

------------------------------------------------------------------------

# Ficha de análisis

## 1. Nombre del Space

**Nombre:** Mage-Flow

**Enlace:** https://huggingface.co/spaces/microsoft/mage-flow

------------------------------------------------------------------------

## 2. ¿Qué hace el agente?

Describa en dos o tres líneas cuál es la función del sistema.

## R/ 

Es un editor y creador de imágenes eficiente con inteligencia artificial con su resolución nativa. Se puede editar una foto por medio de un prompt y elegir si se prefiere rapidez o calidad

------------------------------------------------------------------------

## 3. Análisis PEAS

  Elemento          Respuesta
  ----------------- ----------------------------------------------------
  **Performance**   ¿Qué significa que el agente haga bien su trabajo? Que haga correctamente los cambios descritos en el prompt
  
  **Environment**   ¿Con qué interactúa el agente? La interfaz, el servidor, el modelo de generación de imégenes
  
  **Actuators**     ¿Qué acciones produce? Crear o editar una imágen
  
  **Sensors**       ¿Qué información recibe como entrada? La imágen, el prompt, si se prefiere rapidez o calidad, las configuraciones avanzadas

------------------------------------------------------------------------

## 4. Clasificación del entorno

Complete la siguiente tabla y justifique brevemente cada respuesta.

  Propiedad      Clasificación     Justificación
  -------------- ----------------- ---------------
  Observable     Parcial           No puedo ver el código del modelo de generación pero si su interfaz    
  Determinista   No                No se exactamente como se van a ver los cambios del prompt, hay cierta aleatoriedad si no se es tan específico                       
  Episódico      Sí                Los cambios se hacen a la imagen subida, al tener el resultado y querer añadirle algo se usa el prompt con la imágen original           
  Estático       Sí                El modelo no cambia en cada corrida         
  Discreto       Sí                Crea imágenes y el prompt es texto          
  Conocido       No                El agente solo usa el modelo pero no como exactamente como funciona          

------------------------------------------------------------------------

## 5. ¿Qué tipo de programa de agente creen que es?

Seleccione la opción que consideren más adecuada y explique por qué.

-   Agente de reflejo simple
-   Agente basado en modelo
-   Agente basado en objetivos
-   Agente basado en utilidad
-   Agente con aprendizaje

## R/
Agente basado en modelo: Porque el agente puede ir iterando con su modelo interno de generación de imágenes hasta conseguir el resultado esperado del prompt
> **Importante:** No existe una única respuesta correcta. Lo importante
> es justificar la elección a partir del comportamiento observado.

------------------------------------------------------------------------

# Discusión en clase

Después de las presentaciones, discutiremos preguntas como:

-   ¿Dos Spaces diferentes pueden compartir el mismo tipo de entorno?
-   ¿Es posible saber con certeza qué tipo de agente implementa un Space
    únicamente observándolo?
-   ¿Qué diferencia existe entre el comportamiento observable de un
    agente y su implementación interna?

------------------------------------------------------------------------

# Reto adicional

Encuentre un Space que pueda clasificarse como:

1.  **Totalmente observable, determinista y episódico.**
2.  **Parcialmente observable, estocástico y secuencial.**

Justifique su respuesta.
1. Image Upscaler, cambia la escala de la imágen que suba. Es totalmente observable porque puedo elegir el modelo exacto. Es determinista porque siempre va a escalar el modelo a 1024x1024 y el cambio es solo una imágen a la vez.

2. reachy_mini_conversation_app, un bot conversacional. Es parcialmente observable porque no sabemos nada del modelado interno ni que hace, es estocástico porque no sé con exactitud que va a responder y secuencial porque sigue la conversación.
------------------------------------------------------------------------

# Rúbrica (10 puntos)

| Criterio | Puntos |
|-----------|:------:|
| Descripción correcta del Space | 2 |
| Identificación de PEAS | 3 |
| Clasificación del entorno | 3 |
| Justificación del tipo de agente | 2 |
| **Total** | **10** |

------------------------------------------------------------------------


