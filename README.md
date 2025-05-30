# Apuntes sobre Tablas en HTML

## Introducción
Las tablas en HTML sirven para organizar información en filas y columnas. No se deben usar para crear diseños visuales, sino para presentar datos estructurados.

## Estructura de una Tabla HTML

| Etiqueta   | Descripción                                                  |
|------------|-------------------------------------------------------------|
| `<table>`  | Contenedor general de toda la tabla.                        |
| `<caption>`| Título de la tabla, indica de qué trata.                   |
| `<thead>`  | Sección para los encabezados de columna.                    |
| `<tbody>`  | Parte central, donde van los datos principales.             |
| `<tfoot>`  | Pie de tabla, útil para totales o notas.                   |
| `<tr>`     | Fila de la tabla. Cada `tr` es una línea horizontal.       |
| `<th>`     | Celda de encabezado (usualmente en negrita).               |
| `<td>`     | Celda de datos comunes.                                     |

## Ejemplo Básico de Estructura


## Estilos y Propiedades Útiles

### Estilizando Bordes y Espaciado con CSS

| Propiedad                          | Función                                                  |
|------------------------------------|---------------------------------------------------------|
| `border-collapse: collapse;`      | Junta los bordes de las celdas en una sola línea.      |
| `padding`                          | Espacio interior entre contenido y borde de la celda.   |

### Evitar Estilos Antiguos
Antes se usaban atributos como `cellpadding`, pero ahora se usa CSS moderno para estilos.

### Pseudo-clases para Mejorar la Apariencia

| Pseudo-clase               | Descripción                                           |
|----------------------------|------------------------------------------------------|
| `tr:nth-child(even)`       | Estilo para filas pares (segunda, cuarta...).       |
| `tr:nth-child(odd)`        | Estilo para filas impares (primera, tercera...).    |
| `tr:hover`                 | Aplica un efecto cuando el usuario pasa el cursor sobre una fila. |

## Accesibilidad: `scope` en `<th>`

| Atributo        | Uso                                           |
|------------------|-----------------------------------------------|
| `scope="col"`    | El encabezado aplica a toda la columna.      |
| `scope="row"`    | El encabezado aplica a toda la fila.         |

### Ejemplo


## Buenas Prácticas

- Usar `<caption>` para nombrar la tabla.
- Separar la tabla en `<thead>`, `<tbody>`, y `<tfoot>`.
- Aplicar estilos con CSS, no con atributos antiguos.
- Usar `scope` para mejorar la accesibilidad.
- Nunca usar tablas para maquetar el diseño de la página web.

## Lo que Confirmé en Clase

- Las tablas usan `<table>` como contenedor principal.
- Las filas se crean con `<tr>`.
- Las celdas normales se escriben con `<td>`.
- Las celdas de encabezado se escriben con `<th>`.
- Los bordes por defecto son feos y se deben mejorar con CSS.
- Se pueden aplicar estilos usando pseudo-clases como `nth-child` o `hover`.

## Lo que Aprendí por Mi Cuenta

- `<th>` no es solo decorativo; su uso correcto mejora la accesibilidad.
- Separar la tabla en `<thead>`, `<tbody>` y `<tfoot>` organiza mejor los datos.
- El atributo `scope` en `<th>` ayuda a que los lectores de pantalla interpreten correctamente los encabezados.
- Las tablas son para datos estructurados, no para distribuir visualmente el contenido del sitio.

##Juan Martinez M.