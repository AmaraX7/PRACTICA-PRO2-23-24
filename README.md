# Comercio Fluvial - Práctica PRO2 23-24

Este repositorio contiene la implementación de un sistema de simulación de comercio fluvial entre ciudades situadas en una cuenca hidrográfica, desarrollado como parte de la asignatura **Programación 2 (PRO2)** de la **UPC**.

---

## 📘 Descripción del proyecto

El proyecto simula el comercio de productos entre ciudades ubicadas en una red fluvial, donde:

- Las **ciudades** están situadas en los nacimientos y confluencias de ríos.
- Un **barco** realiza viajes comerciales comprando y vendiendo productos.
- Las ciudades pueden **comerciar entre sí** redistribuyendo productos sobrantes y necesitados.

El sistema implementa todas las operaciones descritas en el enunciado, incluyendo:

- ✅ Gestión de la estructura fluvial y ciudades  
- ✅ Gestión de inventarios de productos  
- ✅ Operaciones comerciales entre ciudades  
- ✅ Planificación de rutas óptimas para el barco comercial  

---

## ⚙️ Requisitos e instalación

### 🧩 Dependencias

Asegúrate de tener las siguientes herramientas instaladas:

```bash
sudo apt install make
sudo apt install g++
sudo apt install doxygen graphviz  # (opcional, para documentación)
````
### 🏗️ Compilación
Navega a la carpeta src:
````bash
cd src
````
Compila el proyecto con make:
````make````

### 🚀 Ejecución

Para ejecutar el programa con un fichero de entrada:

````bash
./program.exe < fichero_input
````
Ejemplo con el fichero de prueba incluido:
````bash
./program.exe < ../samples/sample_completa/sample.inp
````

### 📚 Documentación
Generar documentación con Doxygen
````bash
doxygen Doxyfile
````
Visualizar la documentación generada
````bash
xdg-open DOC/html/index.html
````
### 🧱 Estructura del código

El proyecto sigue una estructura orientada a objetos con las siguientes clases principales:

**Ciudad**: Representa una ciudad con su inventario.

**Producto**: Representa un producto con sus atributos.

**Barco**: Gestiona las operaciones comerciales del barco.

**CuencaFluvial**: Maneja la estructura de la red fluvial y las ciudades.
