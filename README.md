# Detector-Cambios-SHA256-Java
Programa en Java para detectar cambios en archivos utilizando SHA-256.

# 1. ¿Qué hace el programa?
  El programa Detector de cambios en archivos con SHA-256 está desarrollado en Java y tiene como finalidad identificar si un    archivo ha sido modificado desde la última vez que fue registrado.
  Para realizar esta función utiliza el algoritmo criptográfico SHA-256, que genera una huella digital única a partir del contenido de un archivo. Esta huella está formada por 64 caracteres hexadecimales.
Cuando se registra un archivo, el programa calcula su huella SHA-256 y la guarda como referencia. Posteriormente, cuando se desea verificar el archivo, vuelve a calcular su huella y la compara con la que se guardó anteriormente.
Si ambas huellas coinciden, significa que el archivo no ha presentado modificaciones. Si son diferentes, significa que su contenido ha cambiado.
Además, el programa permite consultar los archivos registrados, visualizar un historial de verificaciones, conocer cómo funciona SHA-256 y ejecutar pruebas automáticas para comprobar su funcionamiento.
Funciones principales 
•	Crear y guardar la huella SHA-256 de un archivo.
•	Verificar si un archivo ha cambiado.
•	Mostrar los archivos registrados y sus huellas.
•	Consultar el historial de verificaciones.
•	Explicar cómo funciona SHA-256.
•	Ejecutar pruebas automáticas del programa.
•	Salir del programa.

# 2. ¿Qué se necesita para ejecutar el programa?
Para ejecutar el programa se necesita contar con los siguientes elementos:

## Requisitos del sistema

| Recurso | Descripción |
|---|---|
| Lenguaje de programación | Java. |
| Versión de Java | Java 8 o superior. |
| JDK | Kit de desarrollo de Java para compilar y ejecutar el programa. |
| Editor de código | Visual Studio Code, NetBeans, IntelliJ IDEA o Bloc de notas. |
| Sistema operativo | Windows, Linux o macOS. |
| Memoria RAM | 2 GB como mínimo recomendado para el entorno de desarrollo. |
| Archivos | Código fuente `DetectorSHA256.java`. |

El programa no necesita instalar bibliotecas externas ni tener conexión a Internet, ya que utiliza clases y herramientas incluidas en Java.


## 3. ¿Cómo compilar el programa?

Para compilar el programa, se deben seguir los siguientes pasos:

**Paso 1.** Instalar el JDK de Java en la computadora. Se requiere Java 8 o una versión superior.

**Paso 2.** Guardar el código fuente con el siguiente nombre:

`DetectorSHA256.java`

Es importante que el nombre del archivo coincida exactamente con el nombre de la clase pública del programa.

**Paso 3.** Abrir la terminal o símbolo del sistema y ubicarse en la carpeta donde se encuentra guardado el archivo.

**Paso 4.** Escribir el siguiente comando para compilar:

`javac DetectorSHA256.java`

Este comando permite que el compilador de Java revise el código y, si no encuentra errores, genere un archivo `.class` que contiene el código compilado.

**Paso 5.** Si no aparecen errores, significa que la compilación se realizó correctamente y se habrá generado el archivo:

`DetectorSHA256.class`



## 4. ¿Cómo ejecutar el programa?

Después de compilar el código, se debe ejecutar desde la terminal utilizando el siguiente comando:

`java DetectorSHA256`

Al ejecutarse, aparecerá un menú principal con las siguientes opciones:

| Opción | Función |
|---|---|
| 1 | Crear y guardar la huella de un archivo. |
| 2 | Verificar si un archivo cambió. |
| 3 | Ver archivos registrados. |
| 4 | Consultar el historial de verificaciones. |
| 5 | Consultar información sobre SHA-256. |
| 6 | Ejecutar pruebas automáticas. |
| 0 | Salir del programa. |

El usuario puede seleccionar cualquiera de las opciones escribiendo el número correspondiente y presionando **Enter**.



## 5. ¿Cómo utilizar el programa?

A continuación, se explica cómo utilizar las funciones principales del programa.

### Ejemplo 1. Registrar un archivo

1. Seleccionar la opción **1** del menú principal.
2. Escribir la ruta del archivo que se desea registrar.
3. Presionar **Enter**.
4. El programa calculará la huella digital utilizando el algoritmo SHA-256.
5. Finalmente, mostrará la huella generada y confirmará que fue guardada correctamente.

**Ejemplo de ruta en Windows:**

`C:\Users\Usuario\Documents\prueba.txt`

El programa guardará la ruta del archivo junto con su huella SHA-256 en un archivo llamado:

`manifiesto_sha256.properties`

Este archivo permite conservar las huellas originales para utilizarlas en futuras verificaciones.

### Ejemplo 2. Verificar si un archivo cambió

1. Seleccionar la opción **2** del menú principal.
2. Escribir la ruta del archivo que se desea verificar.
3. El programa calculará nuevamente su huella SHA-256.
4. Comparará la huella actual con la que se registró anteriormente.
5. Mostrará un mensaje indicando el resultado de la comparación.

Se pueden presentar dos resultados:

- **SIN CAMBIOS:** Las huellas coinciden, por lo que no se detectaron modificaciones en el contenido del archivo.
- **MODIFICADO:** Las huellas son diferentes, lo que indica que el contenido del archivo fue modificado.

Para realizar esta verificación, el archivo debe haberse registrado previamente mediante la opción 1.

### Ejemplo 3. Consultar archivos registrados

1. Seleccionar la opción **3** del menú principal.
2. El programa mostrará la lista de archivos que han sido registrados.
3. También mostrará la ruta y la huella SHA-256 correspondiente a cada archivo.

Esta función permite consultar los archivos registrados y conocer las huellas digitales almacenadas en el manifiesto.

### Ejemplo 4. Consultar el historial

1. Seleccionar la opción **4** del menú principal.
2. El programa mostrará las verificaciones realizadas anteriormente.
3. Se podrá consultar la fecha, el resultado de cada verificación y la ruta del archivo.

Esta información se almacena en un archivo llamado:

`historial_sha256.txt`

El historial permite llevar un registro de las verificaciones realizadas durante el uso del programa.

### Ejemplo 5. Ejecutar pruebas automáticas

1. Seleccionar la opción **6** del menú principal.
2. El programa creará archivos temporales para realizar diferentes pruebas.
3. Comprobará el funcionamiento de SHA-256 con archivos pequeños, archivos sin cambios, archivos modificados, archivos grandes y archivos vacíos.
4. Mostrará el resultado de cada prueba mediante los mensajes **OK** o **FALLO**.

Estas pruebas permiten comprobar que el cálculo de las huellas digitales funciona correctamente y que el programa puede detectar modificaciones en los archivos.

## 6. Archivos que genera el programa

Durante su funcionamiento, el programa crea dos archivos principales para almacenar información:

| Archivo | Descripción |
|---|---|
| `manifiesto_sha256.properties` | Guarda las rutas de los archivos registrados junto con sus huellas digitales SHA-256. |
| `historial_sha256.txt` | Almacena las fechas, los resultados de las verificaciones realizadas y las rutas de los archivos. |

Estos archivos se crean automáticamente, cuando se utilizan las funciones correspondientes, en la carpeta desde donde se ejecuta el programa.

El manifiesto permite conservar las huellas originales, mientras que el historial ayuda a consultar los resultados de las verificaciones anteriores.

**Nota:** Es recomendable mantener protegido el archivo del manifiesto, ya que, si alguien modifica tanto el archivo original como su huella guardada, el programa podría no detectar la alteración.
