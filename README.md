# 🎬 Sistema de Gestión de Contenido Audiovisual (POO Java)

Este proyecto es una demostración práctica y robusta de la aplicación de los pilares de la **Programación Orientada a Objetos (POO)** en Java, modelando la gestión de diferentes tipos de contenido audiovisual y sus complejas relaciones.

---

## 🎯 1. Objetivos y Propósito del Proyecto

El objetivo principal de este proyecto es **demostrar la aplicación estructural de la POO** en un dominio complejo.

* **Modelado Jerárquico:** Establecer una jerarquía de clases eficiente, utilizando la **herencia** a partir de una clase abstracta (`ContenidoAudiovisual`) para manejar propiedades comunes.
* **Demostración de Polimorfismo:** Implementar el **polimorfismo** sobrescribiendo el método `mostrarDetalles()` en cada subclase, permitiendo una interacción uniforme.
* **Gestión de Relaciones:** Aplicar **Asociación**, **Composición** y **Agregación** para modelar fielmente las relaciones entre entidades (ej. Series con Temporadas, Películas con Actores).
* **Extensibilidad y Mantenibilidad:** Crear un sistema modular que permita la fácil adición de nuevos tipos de contenido o funcionalidades sin romper la estructura existente.

---

## 🌟 2. Características y Funcionalidades Clave

El sistema implementa conceptos esenciales de POO para modelar el contenido y sus relaciones.

### 2.1. Estructura de Clases Implementadas

| Clase | Tipo | Función Principal y Relaciones |
| :--- | :--- | :--- |
| **`ContenidoAudiovisual`** | Abstracta | Clase base con atributos comunes (título, duración, género). Fuerza el polimorfismo. |
| **`SerieDeTV`** | Concreta | Maneja una colección de objetos `Temporada`. Demuestra **Composición**. |
| **`Pelicula`** | Concreta | Maneja una colección de objetos `Actor`. Demuestra **Asociación**. |
| **`Documental`** | Concreta | Incluye una lista de `Investigador`es y el atributo `temaInvestigado`. |
| **`VideoYouTube`** | Concreta | Atributos específicos como `url` y `numeroDeLikes`. |
| **`Cortometraje`** | Concreta | Similar a `Pelicula`, pero con el atributo `festivalGanado`. |

### 2.2. Mejoras Adicionales Implementadas

* **Optimización POO:** Uso del modificador `final` en atributos clave para asegurar la inmutabilidad y constructores completos para programación defensiva.
* **Gestión Dinámica:** Implementación de `ArrayList` y `List` en las clases de contenido (en lugar de *arrays* fijos) para permitir una gestión dinámica y escalable de elencos y temporadas.
* **Encapsulamiento:** Aplicación estricta del encapsulamiento (`private`) para todos los atributos.

---

## 📊 3. Diagrama de Clases UML

Un diagrama de clases visualiza la estructura de las clases y sus relaciones (herencia, asociación, composición) .

* **Herencia:** Líneas Sólidas con Punta de Flecha.
* **Composición/Agregación:** Líneas Sólidas con Rombo Relleno (Ej. `SerieDeTV` con `Temporada`).
* **Asociación:** Líneas Sólidas Simples (Ej. `Pelicula` con `Actor`).

---

## ⚙️ 4. Tecnologías y Estructura del Proyecto

* **Lenguaje de Programación:** **Java**
* **Entorno de Desarrollo (IDE):** Eclipse IDE
* **Paquetes Principales:**
    * `uni1a/`: Contiene todas las clases del **modelo de dominio**.
    * `poo/`: Contiene la clase principal de ejecución y pruebas (`PruebaAudioVisual.java`).

---

## 🚀 5. Cómo Clonar y Ejecutar el Proyecto

Sigue estos pasos para obtener una copia local del proyecto y ejecutar la demo:

1.  **Clonar el Repositorio:**
    ```bash
    git clone [https://github.com/Past-Alex/POOU2.git](https://github.com/Past-Alex/POOU2.git)
    cd POOU2
    ```

2.  **Importar en Eclipse (o tu IDE de Java preferido):**
    * Abre Eclipse.
    * Ve a `File` > `Import...` > `General` > `Existing Projects into Workspace`.
    * Selecciona la carpeta raíz **`POOU2`** y finaliza la importación.

3.  **Ejecutar el Programa:**
    * Navega hasta la clase `PruebaAudioVisual.java` dentro del paquete `poo`.
    * Haz clic derecho sobre el archivo y selecciona `Run As` > `Java Application`.
    * La salida del programa, que demuestra la creación y el polimorfismo de todos los objetos, se mostrará en la consola.

---

## 🤝 Contribuciones

Si deseas contribuir a este proyecto, por favor sigue el flujo de trabajo estándar de GitHub (Fork, Branch, Commit, Pull Request).

***
