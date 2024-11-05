# XML - Preguntas y Respuestas

### 1. Características propias del lenguaje XML
- **Extensible:** Permite crear etiquetas personalizadas según las necesidades del usuario.
- **Auto-descriptivo:** Cada dato se acompaña de una etiqueta que lo describe.
- **Jerárquico:** Los datos se organizan en una estructura en árbol.
- **Legible por humanos y máquinas:** Está diseñado para ser fácilmente comprensible tanto por humanos como por computadoras.
- **Plataforma independiente:** Es un estándar universal que puede ser interpretado en diferentes sistemas operativos y aplicaciones.
- **Bien formado y válido:** Un documento XML debe cumplir con ciertas reglas de sintaxis (bien formado) y, opcionalmente, con un esquema o DTD que valide su estructura y contenido.

### 2. Estructura de un documento XML y reglas sintácticas
La estructura básica de un documento XML consta de:
- **Declaración XML:** `<?xml version="1.0" encoding="UTF-8"?>` que especifica la versión y la codificación.
- **Elemento raíz (nodo raíz):** Todos los elementos deben estar contenidos dentro de un único elemento raíz.
- **Elementos y atributos:** Los datos se representan mediante etiquetas y atributos. Los atributos proporcionan información adicional sobre los elementos.
- **Jerarquía en árbol:** Los elementos pueden contener otros elementos formando una jerarquía.
- **Reglas sintácticas:**
  - Los elementos deben estar correctamente anidados.
  - Todos los elementos deben tener una etiqueta de apertura y cierre o ser auto-cerrados (`<elemento/>`).
  - Los nombres de los elementos son sensibles a mayúsculas y minúsculas.
  - Las comillas en los atributos deben ser consistentes (usualmente dobles).

### 3. ¿Qué es un nodo raíz en XML?
El nodo raíz es el primer elemento que contiene a todos los demás elementos del documento XML. Es obligatorio y debe haber solo uno por documento. En el siguiente ejemplo, `<restaurante>` es el nodo raíz:
``xml
<restaurante>
    <!-- Otros elementos -->
</restaurante>

## 4¿Qué es un elemento vacío? Ejemplos
Un elemento vacío es un elemento sin contenido. Puede escribirse como:

<plato></plato>

## 5. Importancia de crear documentos XML bien formados
Facilita la correcta interpretación de los datos por cualquier procesador XML.
Asegura interoperabilidad y facilita la validación contra esquemas o DTDs.

## 6. ¿Qué es un espacio de nombres? Ventajas
Un espacio de nombres evita conflictos de etiquetas en un documento XML combinando vocabularios diferentes. Se define mediante un prefijo y una URI única.

Ventajas:

- Evita colisiones de nombres.
- Permite reutilizar etiquetas en distintos contextos.

## 7. Entidades en XML
Representan caracteres especiales que no se pueden escribir directamente. Ejemplos:

&lt; para <
&gt; para >
&amp; para &
## 8. Comentarios en XML
Los comentarios en XML no son procesados por el parser y se encierran entre <!-- y -->.

ejemplo:
<!--
<restaurante nombre="Grande es el Capitán">
    <contacto>
        <telefono>678123456</telefono>
    </contacto>
</restaurante>
-->