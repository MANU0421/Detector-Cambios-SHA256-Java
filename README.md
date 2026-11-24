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


