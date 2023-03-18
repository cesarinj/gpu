
## Resolucion de examen  GPU
Este repositorio contiene la resolucion del examen del curso Computacion de alto rendimiento con GPUs 
Dictado por Leonardo y Luciana


El objetivo de la presente evaluacion es poder verificar un codigo ejemplo con VT Tune Y Advisor , herramients de intel ( herramientas que nos permiten poder decir que tan paralelisable es , si es mejor usar GPUs o CPUs


escrito por cesar aguirre

## 0. Clonar el repositorio [`oneAPI-samples`](https://github.com/oneapi-src/oneAPI-samples) [1 punto]

![clonacion](https://github.com/cesarinj/gpu/blob/main/clonacion.JPG)

https://github.com/cesarinj/gpu/blob/main/clonacion.JPG

En este paso se tomara un ejemplo de ONeAPI, nosotros usaremos nbody
clonacion de repositorio



## 2. Cambiar al directorio del ejemplo `Nbody`  [1 punto]
    - Directorio: `oneAPI-samples/tree/master/DirectProgramming/C++SYCL/N-BodyMethods/Nbody`


![carpeta](https://github.com/cesarinj/gpu/blob/main/carpeta.JPG)

en este carpeta se muestra los archivos que contiene la carpeta nbody

## 3. Explicar brevemente el algoritmo de `Nbody` [3 puntos]

La simulación de Nbody es una simulación de un sistema dinámico de partículas,que se encuentran interaccionando por las fuerzas como la gravedad. Este código de muestra de Nbody usa estándares SYCL* para CPU y GPU.


## 4. Acceder en modo interactivo a un nodo de cómputo con GPUs (`gen9` o `gen11`) [3 puntos]
    - Compilar y ejecutar `Nbody`
    - Proporcionar screenshot(s) de los resultados

![make](https://github.com/cesarinj/gpu/blob/main/make.JPG)
En este grafico se compila creando una carpeta de trabajo nbody


![carpeta](https://github.com/cesarinj/gpu/blob/main/1.jpg)
Simulacion de gravedad


![carpeta](https://github.com/cesarinj/gpu/blob/main/2.jpg)


![carpeta](https://github.com/cesarinj/gpu/blob/main/3.jpg)


![carpeta](https://github.com/cesarinj/gpu/blob/main/4.jpg)


        - Por cada screenshot, añadir una breve descripción
## 5. Realizar un análisis de _**GPU Hotspots**_ con VTune [8 puntos]
Nos permite ver mejoras que se pueden dar en la arquitetura 


    - Indicar los hotspots del programa
    - Proporcionar screenshot(s) de los resultados
      - Por cada screenshot, añadir una breve descripción


![carpeta](https://github.com/cesarinj/gpu/blob/main/vttune.jpg)

## 6. Realizar un análisis _**Roofline**_ con Advisor [4 puntos]

    - Indicar los hotspots del programa
    - Proporcionar screenshot(s) de los resultados
      - Por cada screenshot, añadir una breve descripción
    - Indicar potenciales soluciones para optimizar la ejecución del programa
 
 
 Mejora de codigo
 memory bound alta dependencia de acceso de memoria
 compute bound el cuello de botella se debe a que queremos porque queremos usar muchas operaciones sistematicamnte
    
![rutinas](https://github.com/cesarinj/gpu/blob/main/rutinas.jpg)
Nos muesta que podemos tener mas mejoras or acceso a memoria que por problemas de hardware 
![carpeta](https://github.com/cesarinj/gpu/blob/main/5.jpg)
![carpeta](https://github.com/cesarinj/gpu/blob/main/6.jpg)
