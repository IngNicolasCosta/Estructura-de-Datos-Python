# Implementación de Estructuras de Datos en Python 🐍

Este repositorio contiene la implementación desde cero de estructuras de datos lineales fundamentales utilizando **Python**. El objetivo de este proyecto es demostrar la comprensión profunda de la lógica algorítmica, el manejo de referencias (punteros) y la manipulación de nodos en memoria.

## 📂 Contenido del Repositorio

El proyecto consta de dos implementaciones principales de listas enlazadas, diseñadas con Programación Orientada a Objetos (POO).

### 1. Lista Doblemente Enlazada (`lista doble enlazada.py`)
Una estructura de datos lineal donde cada nodo tiene referencias tanto al nodo siguiente como al anterior, permitiendo un recorrido bidireccional eficiente.

**Clase `Nodo`:** Almacena el `dato`, un puntero `siguiente` y un puntero `anterior`.
**Funcionalidades Implementadas:**
    **Inserción:** Métodos `agregar_inicio` y `agregar_final` que actualizan dinámicamente los punteros de cabecera y cola.
    **Eliminación:** Métodos `eliminar_primero` y `eliminar_ultimo` con manejo de casos borde (listas vacías o de un solo elemento) y limpieza de referencias.
    **Recorrido:** Capacidad de imprimir la lista en orden ascendente (`printear_inicio_lista`) y descendente (`printear_final_lista`).

### 2. Lista Circular Simple (`Lista Circular.py`)
Una variación de la lista enlazada donde el último nodo apunta de regreso al primero, creando un ciclo continuo. Ideal para aplicaciones que requieren iteración continua (como buffers circulares).

**Clase `Nodo`:** Estructura simple con `dato` y puntero `siguiente`.
**Funcionalidades Implementadas:**
    **Lógica Circular:** Garantiza que `self.ultimo.siguiente` siempre apunte a `self.primero` tras cada inserción o eliminación.
    **Gestión de Punteros:** Métodos `agregarinicio` y `agregarfinal` que mantienen la integridad del ciclo.
    **Recorrido Controlado:** El método `printear` incluye lógica específica para detenerse al completar una vuelta completa al ciclo, evitando bucles infinitos al imprimir.

## 🛠️ Tecnologías y Conceptos Aplicados

**Lenguaje:** Python 3.x
**Paradigmas:** Programación Orientada a Objetos (Clases, Objetos, Métodos).
**Estructuras de Datos:** Listas Enlazadas (Linked Lists).
**Algoritmos:** Inserción y borrado en O(1) (para extremos) y recorrido en O(n).

## 🚀 Cómo ejecutar el código

Asegúrate de tener Python instalado. Puedes ejecutar cada archivo individualmente para ver las pruebas de escritorio incluidas en el `main`:

```bash
# Para ejecutar la Lista Doblemente Enlazada
python "lista doble enlazada.py"

# Para ejecutar la Lista Circular
python "Lista Circular.py"
