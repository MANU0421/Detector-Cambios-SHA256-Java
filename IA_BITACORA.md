# Bitácora de uso de Inteligencia Artificial

## Registro 1. Análisis técnico del código fuente

**Tipo de registro:** Revisión del código.

**Instrucción proporcionada a la IA:** Analizar el código fuente del programa Detector de cambios en archivos con SHA-256 y explicar su funcionamiento general.

**Aportación de la IA:** La IA explicó la estructura del programa, sus principales métodos y las funciones que realiza cada opción del menú.

**Verificación del equipo:** Se revisó el código fuente y se compararon las explicaciones con las instrucciones implementadas en el programa.

**Resultado:** Se obtuvo una mejor comprensión de la estructura y funcionamiento del sistema.

---

## Registro 2. Evaluación del algoritmo SHA-256

**Tipo de registro:** Análisis criptográfico.

**Instrucción proporcionada a la IA:** Explicar cómo funciona SHA-256 y cómo se utiliza para identificar cambios en los archivos.

**Aportación de la IA:** La IA explicó que SHA-256 genera una huella digital única a partir del contenido de un archivo. Cuando el contenido cambia, también cambia su huella.

**Verificación del equipo:** Se revisó el método `calcularSHA256()` y se realizaron comparaciones entre las huellas de archivos.

**Resultado:** Se comprendió la importancia del algoritmo para detectar modificaciones en los archivos.

---

## Registro 3. Almacenamiento y persistencia de información

**Tipo de registro:** Revisión del almacenamiento de datos.

**Instrucción proporcionada a la IA:** Explicar cómo se guardan los registros de los archivos y los resultados de las verificaciones.

**Aportación de la IA:** La IA identificó el uso de `manifiesto_sha256.properties` para almacenar las rutas y huellas digitales, así como `historial_sha256.txt` para conservar los resultados de las verificaciones.

**Verificación del equipo:** Se revisó la creación y actualización de ambos archivos durante la ejecución del programa.

**Resultado:** Se identificó cómo el sistema conserva la información para futuras consultas.

---

## Registro 4. Manejo de errores y excepciones

**Tipo de registro:** Evaluación del manejo de errores.

**Instrucción proporcionada a la IA:** Identificar posibles errores que podrían presentarse al utilizar el programa y proponer pruebas para comprobar su comportamiento.

**Aportación de la IA:** La IA propuso probar rutas inexistentes, campos vacíos y archivos que todavía no estuvieran registrados.

**Verificación del equipo:** Se revisaron las validaciones del código y se realizaron las pruebas correspondientes para observar las respuestas del programa.

**Resultado:** Se identificaron situaciones que permiten evaluar la respuesta del sistema ante entradas incorrectas.

---

## Registro 5. Diseño de pruebas de software

**Tipo de registro:** Planeación de pruebas.

**Instrucción proporcionada a la IA:** Proponer casos de prueba para comprobar que las funciones principales del programa trabajen correctamente.

**Aportación de la IA:** La IA propuso pruebas con archivos pequeños, archivos vacíos, archivos modificados y archivos de mayor tamaño, además de verificar archivos sin cambios.

**Verificación del equipo:** Se ejecutaron las pruebas disponibles en el programa y se revisaron los resultados obtenidos.

**Resultado:** Se estableció un conjunto de pruebas para evaluar el funcionamiento del sistema en diferentes situaciones.

---

## Registro 6. Análisis de seguridad y limitaciones

**Tipo de registro:** Evaluación de seguridad.

**Instrucción proporcionada a la IA:** Analizar la utilidad de SHA-256 para detectar modificaciones y señalar las limitaciones del programa.

**Aportación de la IA:** La IA explicó que SHA-256 permite identificar cambios en el contenido de los archivos, pero que el programa no impide que estos sean modificados. También señaló que el manifiesto debe protegerse para evitar alteraciones no autorizadas.

**Verificación del equipo:** Se revisaron las funciones implementadas y se compararon con las recomendaciones proporcionadas.

**Resultado:** Se identificaron las ventajas y limitaciones del sistema, así como posibles mejoras de seguridad.

---

# Reflexión final

La inteligencia artificial fue una herramienta de apoyo durante el desarrollo y análisis del programa Detector de cambios en archivos con SHA-256. Permitió comprender mejor el funcionamiento del código, conocer la utilidad del algoritmo criptográfico, identificar posibles errores y proponer pruebas para evaluar el sistema.

Sin embargo, las respuestas de la IA no se tomaron como resultados definitivos. El equipo revisó el código fuente, comprobó las funciones implementadas y verificó el comportamiento del programa mediante su ejecución. Esto permitió distinguir entre las características que realmente tiene el sistema y las recomendaciones que podrían considerarse como mejoras futuras.

En conclusión, la inteligencia artificial facilitó el proceso de análisis y documentación, pero la responsabilidad de comprobar que la información fuera correcta y que el programa funcionara adecuadamente correspondió al equipo de trabajo.
