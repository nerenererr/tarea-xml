# Tarea 1: Fundamentos de XML - Catálogo de Manga

Este repositorio contiene la solución a la **Tarea 1** de la asignatura de Lenguajes de Marcas. El objetivo del proyecto es ayudar a **Felipe** a estructurar una base de datos inicial para su futura página web sobre manga y anime.

## 📖 Descripción del Proyecto

Se ha diseñado un documento XML estandarizado que almacena información detallada sobre colecciones de cómics japoneses. El documento cumple con los estándares del W3C para documentos **bien formados** y utiliza **Espacios de Nombres (Namespaces)** para organizar la información semánticamente.

### Obras Incluidas
El archivo XML contiene el registro detallado de dos obras icónicas:
1.  **NANA** (Ai Yazawa) - *Género Josei*
2.  **Berserk** (Kentaro Miura) - *Género Seinen*

## 🛠️ Tecnologías y Conceptos Aplicados

En este proyecto se han puesto en práctica los siguientes conceptos:

* **XML Bien Formado:**
    * Existencia de un único elemento raíz (`<coleccion>`).
    * Correcto anidamiento de etiquetas.
    * Cierre de todas las etiquetas abiertas.
    * Uso de comillas en todos los atributos.
* **Espacios de Nombres (Namespaces):**
    * Se han creado prefijos para diferenciar el vocabulario y evitar conflictos de nombres (por ejemplo, diferenciar el nombre del manga del nombre del autor).


## 🚀 Cómo Validar el XML

Para verificar que el código no tiene errores de sintaxis:

1.  **Navegador Web:** Arrastra el archivo `coleccion_manga.xml` a cualquier navegador (Chrome, Firefox, Edge). Si el archivo es válido, verás el árbol de etiquetas coloreado. Si hay un error, el navegador mostrará un mensaje de alerta.
2.  **Validador Online:** Puedes copiar el contenido y pegarlo en herramientas como [XMLValidation.com](https://www.xmlvalidation.com/).

## Validación
<img width="1025" height="574" alt="Captura de pantalla 2026-02-03 140339" src="https://github.com/user-attachments/assets/136dfd34-ffe0-44f4-aaa3-512c1259e388" />

## 📝 Ejemplo de Código

A continuación se muestra un fragmento de cómo se estructura una obra dentro del archivo:

```xml
<manga:obra id="002" tipo="seinen">
    <manga:titulo idioma="español">Berserk</manga:titulo>
    <editorial:publicacion>
        <editorial:autor>
            <persona:nombre>Kentaro Miura</persona:nombre>
        </editorial:autor>
    </editorial:publicacion>
</manga:obra>


