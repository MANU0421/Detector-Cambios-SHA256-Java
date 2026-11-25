Proyecto: Detector de cambios en archivos con SHA-256.
Herramienta utilizada: ChatGPT.
Registro 1. Análisis técnico del código fuente
Tipo de registro: Análisis técnico.

Instrucción proporcionada a la IA:

Analiza el código fuente del programa Detector de cambios en archivos con SHA-256. Identifica la función de sus métodos principales, las bibliotecas utilizadas y la relación entre sus componentes. Explica cómo se organiza el programa y cuál es el propósito de cada una de sus funciones.

Aportación de la IA: Explicó la estructura del programa y la función de los métodos principales, facilitando la comprensión de su funcionamiento.

Verificación del equipo: Se revisaron los métodos directamente en el código para confirmar que las explicaciones fueran correctas.

Resultado: Se comprendió la organización y funcionamiento general del programa.

Registro 2. Evaluación del algoritmo SHA-256
Tipo de registro: Análisis criptográfico.

Instrucción proporcionada a la IA:

Explica cómo se implementa SHA-256 en el programa, cómo se generan las huellas digitales y cómo se utilizan para detectar modificaciones en los archivos. Describe también la importancia de este algoritmo para garantizar la integridad de la información.

Aportación de la IA: Explicó el proceso de generación de huellas digitales y la comparación de resultados para identificar cambios.

Verificación del equipo: Se revisó el método calcularSHA256() y se comprobó que generara huellas de 64 caracteres hexadecimales.

Resultado: Se comprendió la importancia de SHA-256 en la detección de modificaciones.

Registro 3. Almacenamiento y persistencia de información
Tipo de registro: Análisis de almacenamiento de datos.

Instrucción proporcionada a la IA:

Identifica cómo el programa almacena las huellas digitales y los resultados de las verificaciones. Explica la función del manifiesto y del archivo de historial, así como la manera en que se recupera la información cuando el programa vuelve a ejecutarse.

Aportación de la IA: Describió la función de los archivos manifiesto_sha256.properties e historial_sha256.txt y los mecanismos utilizados para guardar la información.

Verificación del equipo: Se revisaron los métodos de lectura y escritura y se comprobó la creación de los archivos correspondientes.

Resultado: Se identificó cómo se conserva la información entre diferentes ejecuciones.

Registro 4. Manejo de errores y excepciones
Tipo de registro: Evaluación de errores.

Instrucción proporcionada a la IA:

Examina las validaciones del programa e identifica cómo responde ante rutas inexistentes, entradas vacías, archivos no registrados y problemas de lectura. Explica la función de las excepciones utilizadas y propone pruebas para comprobar su funcionamiento.

Aportación de la IA: Identificó los mecanismos de validación existentes y propuso diferentes escenarios para evaluar el manejo de errores.

Verificación del equipo: Se revisaron los métodos de validación y se realizaron pruebas con rutas incorrectas y archivos no registrados.

Resultado: Se comprobó el comportamiento del programa ante diferentes situaciones de error.

Registro 5. Diseño de pruebas de software
Tipo de registro: Planificación de pruebas.

Instrucción proporcionada a la IA:

Diseña un conjunto de pruebas para evaluar el funcionamiento del programa, incluyendo el registro de archivos, detección de modificaciones, archivos vacíos, archivos grandes y situaciones de error. Describe los pasos y resultados esperados de cada prueba.

Aportación de la IA: Propuso diferentes escenarios de prueba y explicó cómo evaluar los resultados obtenidos.

Verificación del equipo: Se ejecutaron las pruebas desde Visual Studio Code y se compararon los resultados con los comportamientos esperados.

Resultado: Se establecieron pruebas para evaluar el funcionamiento y la confiabilidad del programa.

Registro 6. Análisis de seguridad y limitaciones
Tipo de registro: Evaluación de seguridad informática.

Instrucción proporcionada a la IA:

Analiza las capacidades y limitaciones del programa respecto a la seguridad de los archivos. Explica qué sucede si se modifica un archivo y también su manifiesto, diferencia integridad de autenticidad y proporciona recomendaciones para fortalecer el sistema.

Aportación de la IA: Explicó que SHA-256 permite detectar modificaciones, pero que el manifiesto también podría alterarse, por lo que el sistema tiene limitaciones de seguridad.

Verificación del equipo: Se revisó el mecanismo de almacenamiento de las huellas y se comprobó que no existe una protección adicional del manifiesto.

Resultado: Se identificaron las limitaciones del programa y posibles mejoras de seguridad.
