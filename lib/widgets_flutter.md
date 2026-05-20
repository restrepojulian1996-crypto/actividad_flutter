# Investigación de widgets fundamentales en Flutter

**Nombre del estudiante:** Julián David Restrepo Montes  
**Curso:** Lenguajes de programacion para la web  
**Fecha:** 18/05/2026

## 1. `Container`

### Descripción

El widget `Container` es uno de los widgets más utilizados en Flutter. Se usa para crear cajas visuales que permiten organizar y personalizar otros widgets dentro de la interfaz.

Este widget es útil para modificar tamaños, colores, márgenes, rellenos y alineaciones.

### Ejemplo de código

```dart
Container(
  width: 200,
  height: 100,
  color: Colors.blue,
  alignment: Alignment.center,
  child: Text(
    'Hola Flutter',
    style: TextStyle(
      color: Colors.white,
      fontSize: 20,
    ),
  ),
)
```

### Explicación del ejemplo

En este ejemplo se crea un contenedor azul con un texto centrado en color blanco.

El `Container` tiene un ancho de 200 píxeles y una altura de 100 píxeles.

### Personalización

| Propiedad | Descripción |
|---|---|
| `width` | Define el ancho |
| `height` | Define la altura |
| `color` | Cambia el color |
| `alignment` | Alinea el contenido |
| `padding` | Agrega espacio interno |
| `margin` | Agrega espacio externo |

### Ejemplo con personalización

```dart
Container(
  width: 250,
  height: 120,
  padding: EdgeInsets.all(20),
  margin: EdgeInsets.all(10),
  alignment: Alignment.center,
  decoration: BoxDecoration(
    color: Colors.green,
    borderRadius: BorderRadius.circular(15),
  ),
  child: Text(
    'Container personalizado',
    style: TextStyle(
      color: Colors.white,
      fontSize: 18,
    ),
  ),
)
```

### Conclusión

El widget `Container` es fundamental porque permite organizar y personalizar elementos visuales dentro de una aplicación Flutter.



## 2. `Text`

### Descripción

El widget `Text` se utiliza para mostrar texto en pantalla dentro de una aplicación Flutter.

Es uno de los widgets más importantes porque permite mostrar títulos, mensajes, descripciones, botones y cualquier tipo de información escrita para el usuario.

Además, el widget `Text` permite personalizar el color, tamaño, alineación y estilo del texto.

### Ejemplo de código

```dart
Text(
  'Hola Flutter',
)
```

### Explicación del ejemplo

En este ejemplo, el widget `Text` muestra el mensaje `Hola Flutter` en la pantalla.

Es la forma más sencilla de mostrar texto en Flutter.

### Personalización

| Propiedad | Descripción |
|---|---|
| `style` | Permite modificar el diseño del texto |
| `textAlign` | Alinea el texto |
| `maxLines` | Define el número máximo de líneas |
| `overflow` | Controla el desbordamiento del texto |
| `softWrap` | Permite dividir líneas automáticamente |

### Ejemplo con personalización

```dart
Text(
  'Texto personalizado en Flutter',
  textAlign: TextAlign.center,
  style: TextStyle(
    color: Colors.blue,
    fontSize: 24,
    fontWeight: FontWeight.bold,
    fontStyle: FontStyle.italic,
  ),
)
```

### Explicación de la personalización

En este ejemplo, el texto aparece centrado, con color azul, tamaño grande, negrita y estilo cursiva.

La propiedad `TextStyle` permite modificar visualmente el texto para hacerlo más atractivo y fácil de leer.

### Conclusión

El widget `Text` es fundamental en Flutter porque permite mostrar información al usuario de manera clara y personalizada.


    ## 3. `Row`

### Descripción

El widget `Row` se utiliza para organizar varios widgets horizontalmente en una misma fila.

Es útil para crear menús, botones alineados, íconos con texto y distribuciones horizontales dentro de la interfaz.

### Ejemplo de código

```dart
Row(
  children: [
    Icon(Icons.star),
    Text('Favorito'),
  ],
)
```

### Explicación del ejemplo

En este ejemplo, el widget `Row` organiza un ícono y un texto en una misma línea horizontal.

La propiedad `children` permite agregar múltiples widgets dentro del `Row`.

### Personalización

| Propiedad | Descripción |
|---|---|
| `children` | Lista de widgets hijos |
| `mainAxisAlignment` | Alinea horizontalmente |
| `crossAxisAlignment` | Alinea verticalmente |
| `mainAxisSize` | Controla el tamaño horizontal |

### Ejemplo con personalización

```dart
Row(
  mainAxisAlignment: MainAxisAlignment.spaceEvenly,
  crossAxisAlignment: CrossAxisAlignment.center,
  children: [
    Icon(Icons.home),
    Icon(Icons.search),
    Icon(Icons.settings),
  ],
)
```

### Explicación de la personalización

En este ejemplo, los íconos aparecen distribuidos uniformemente gracias a `spaceEvenly`.

El widget `Row` ayuda a construir interfaces organizadas horizontalmente.

### Conclusión

El widget `Row` es importante porque permite distribuir widgets en filas de manera organizada y flexible.




## 4. `Column`

### Descripción

El widget `Column` se utiliza para organizar widgets verticalmente en una columna.

Es muy útil para construir formularios, menús, listas simples y estructuras verticales dentro de una aplicación Flutter.

El widget `Column` permite colocar varios elementos uno debajo del otro.

### Ejemplo de código

```dart
Column(
  children: [
    Text('Nombre'),
    Text('Correo'),
    Text('Teléfono'),
  ],
)
```

### Explicación del ejemplo

En este ejemplo, el widget `Column` organiza tres textos de manera vertical.

Cada widget aparece debajo del anterior gracias a la propiedad `children`.

### Personalización

| Propiedad | Descripción |
|---|---|
| `children` | Lista de widgets hijos |
| `mainAxisAlignment` | Alinea verticalmente |
| `crossAxisAlignment` | Alinea horizontalmente |
| `mainAxisSize` | Controla el tamaño vertical |

### Ejemplo con personalización

```dart
Column(
  mainAxisAlignment: MainAxisAlignment.center,
  crossAxisAlignment: CrossAxisAlignment.start,
  children: [
    Text('Flutter'),
    Text('Widgets'),
    Text('Column'),
  ],
)
```

### Explicación de la personalización

En este ejemplo, los textos aparecen centrados verticalmente y alineados a la izquierda.

Las propiedades de alineación ayudan a organizar mejor los elementos dentro de la interfaz.

### Conclusión

El widget `Column` es fundamental porque permite organizar widgets verticalmente de forma clara y estructurada.



## 5. `ElevatedButton`

### Descripción

El widget `ElevatedButton` se utiliza para crear botones interactivos en Flutter.

Los botones permiten que el usuario realice acciones dentro de la aplicación, como enviar formularios, navegar entre pantallas o ejecutar funciones.

Este widget incluye un diseño moderno con elevación y color de fondo.

### Ejemplo de código

```dart
ElevatedButton(
  onPressed: () {
    print('Botón presionado');
  },
  child: Text('Presionar'),
)
```

### Explicación del ejemplo

En este ejemplo, el botón muestra el texto `Presionar`.

Cuando el usuario hace clic sobre el botón, se ejecuta la función `print`.

La propiedad `onPressed` define la acción que realizará el botón.

### Personalización

| Propiedad | Descripción |
|---|---|
| `onPressed` | Acción del botón |
| `child` | Contenido interno |
| `style` | Personaliza el diseño |
| `icon` | Agrega íconos |
| `enabled` | Habilita o deshabilita el botón |

### Ejemplo con personalización

```dart
ElevatedButton(
  onPressed: () {},
  style: ElevatedButton.styleFrom(
    backgroundColor: Colors.green,
    padding: EdgeInsets.symmetric(
      horizontal: 30,
      vertical: 15,
    ),
  ),
  child: Text(
    'Guardar',
    style: TextStyle(
      fontSize: 18,
      color: Colors.white,
    ),
  ),
)
```

### Explicación de la personalización

En este ejemplo, el botón tiene color verde, mayor tamaño y texto personalizado.

La propiedad `styleFrom` permite modificar fácilmente la apariencia del botón.

### Conclusión

El widget `ElevatedButton` es importante porque permite crear interacciones entre el usuario y la aplicación mediante botones modernos y personalizables.