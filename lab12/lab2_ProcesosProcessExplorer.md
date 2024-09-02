# Tarea: Procesos - Process Explorer

Para la realización de las siguientes prácticas deberemos instalar en el Sistema la herramienta Process Explorer:

[Process Explorer](https://docs.microsoft.com/en-us/sysinternals/downloads/process-explorer#download)

Se trata de un software desarrollado por SysInternals y que fué comprado por Microsoft y ahora se ofrece de manera gratuita desde la página de Microsoft.

## Ejercicio 1

Lanza el Bloc de Notas y el Edge, abre el Process Explorer y comprueba que los procesos han sido lanzados y están en marcha.

Realiza una captura de pantalla.
![Alt text](image-5.png)

## Ejercicio 2

Utilizando la opción de menú *Propiedades* sobre notepad.exe, obtén los siguientes datos acerca del ejecutable del Bloc de Notas.

![Alt text](image-6.png)


* Path: C:\Windows\System32\notepad.exe
* Linea de ejecución: "C:\Windows\system32\notepad.exe" 
* Directorio actual: C:\Users\groitomy\
* Usuario que lo ha lanzado: DESKTOP-IL13DT6\groitomy
* Proceso que lo ha lanzado (padre): explorer.exe(8368)
* Versión: 10.0.190.41.488

## Ejercicio 3

Obtén los mismos datos de 4 programas conocidos. Puedes realizar esta tarea en casa.

![Alt text](image-7.png)

* Path: C:\Windows\explorer.exe
* Linea de ejecución: C:\Windows\Explorer.EXE
* Directorio actual: C:\Windows\System32\
* Usuario que lo ha lanzado: DESKTOP-IL13DT6\groitomy
* Proceso que lo ha lanzado (padre): none
* Versión: 10.0.19041.610

![Alt text](image-8.png)

* Path: C:\Windows\System32\MicrosoftEdgeCP.exe
* Linea de ejecución: "C:\Windows\System32\MicrosoftEdgeCP.exe" -ServerName:Windows.Internal.WebRuntime.ContentProcessServer
* Directorio actual: C:\Windows\SystemApps\Microsoft.MicrosoftEdge_8wekyb3d8bbwe\
* Usuario que lo ha lanzado: DESKTOP-IL13DT6\groitomy
* Proceso que lo ha lanzado (padre): none
* Versión: 11.0.19041.1

![Alt text](image-9.png)

* Path: C:\Program Files\WindowsApps\Microsoft.WindowsCalculator_10.1906.55.0_x64__8wekyb3d8bbwe\Calculator.exe
* Linea de ejecución: "C:\Program Files\WindowsApps\Microsoft.WindowsCalculator_10.1906.55.0_x64__8wekyb3d8bbwe\Calculator.exe" -ServerName:App.AppXsm3pg4n7er43kdh1qp4e79f1j7am68r8.mca
* Directorio actual: C:\Program Files\WindowsApps\Microsoft.WindowsCalculator_10.1906.55.0_x64__8wekyb3d8bbwe\
* Usuario que lo ha lanzado: DESKTOP-IL13DT6\groitomy
* Proceso que lo ha lanzado (padre): none
* Versión: 10.1906.55.0

![Alt text](image-10.png)

* Path: C:\Windows\regedit.exe
* Linea de ejecución: "C:\Windows\regedit.exe" 
* Directorio actual: C:\Windows\System32\
* Usuario que lo ha lanzado: DESKTOP-IL13DT6\groitomy
* Proceso que lo ha lanzado (padre): explorer.exe(8368)
* Versión: 10.0.19041.1