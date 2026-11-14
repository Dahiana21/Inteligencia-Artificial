
## Ejercicio · Mostrar tres números de menor a mayor

El objetivo fue mostrar tres números en orden ascendente. Para resolverlo, comparé los valores de `a`, `b` y `c` con condicionales. Las variables conservan sus valores originales. Lo que cambia es el orden en el que las escribo en `console.log()`.

### Código

```javascript
let a = 10;
let b = 5;
let c = 20;

if (a <= b && b <= c) {
    console.log(a, b, c);
} else if (a <= c && c <= b) {
    console.log(a, c, b);
} else if (b <= a && a <= c) {
    console.log(b, a, c);
} else if (b <= c && c <= a) {
    console.log(b, c, a);
} else if (c <= a && a <= b) {
    console.log(c, a, b);
} else {
    console.log(c, b, a);
}
```

### Cómo funciona

1. **Guardo los números.** Con `let` declaro tres variables. En este ejemplo, `a` vale `10`, `b` vale `5` y `c` vale `20`.
2. **Comparo los valores.** El operador `<=` significa «menor o igual que». Por ejemplo, `b <= a` pregunta si `5` es menor o igual que `10`. Usar `<=` también permite trabajar con números repetidos.
3. **Compruebo un orden completo.** El operador `&&` significa «y». En `b <= a && a <= c` deben cumplirse ambas comparaciones. Así compruebo que `b` puede ir primero, `a` en el medio y `c` al final.
4. **Muestro el resultado.** JavaScript revisa las condiciones de arriba hacia abajo. En cuanto encuentra la primera verdadera, ejecuta su `console.log()` y termina la cadena de decisiones. Si las cinco condiciones son falsas, el `else` muestra el orden restante: `c, b, a`.

### Qué pasa con los valores del ejemplo

| `a <= b && b <= c` | ¿Está `10, 5, 20` en orden? | Falso. `10` es mayor que `5`. |
| `a <= c && c <= b` | ¿Está `10, 20, 5` en orden? | Falso. `20` es mayor que `5`. |
| `b <= a && a <= c` | ¿Está `5, 10, 20` en orden? | Verdadero. Se ejecuta `console.log(b, a, c)`. |

La consola muestra:

```text
5 10 20
```

## Actividad · Tres cupos, ocho estudiantes

En esta actividad comparé mi decisión con dos respuestas de una inteligencia artificial. El caso era ficticio: ocho estudiantes de programación tenían distintas notas, porcentajes de asistencia y dificultades para aprender, pero solo había tres cupos para un programa de acompañamiento.

### Mi elección y las dos consultas

| Mi elección individual | Elena, Camila y Ana | Tomé la asistencia como indicador de compromiso y participación. Elena y Camila asistían al 100 % de las clases y Ana al 95 %. |
| Primera consulta a la IA | Diego, Ana y Gabriela | Le pedí que eligiera a quienes más necesitaban acompañamiento y justificara tanto las elecciones como las exclusiones. La IA tuvo en cuenta las notas, las dificultades de aprendizaje y las circunstancias de cada estudiante. |
| Segunda consulta a la IA | Diego, Gabriela y Ana | Repetí la pregunta con los mismos datos y añadí la descripción del Programa B. La IA explicó cómo los recursos disponibles podían ayudar a cada estudiante a continuar en el curso. |

### Qué cambió al agregar el Programa B

El **Programa B** buscaba evitar el abandono del curso. Ofrecía ocho semanas de acompañamiento con tutorías en horarios flexibles y seis horas adicionales de acceso a un computador por semana.

La IA eligió a **las mismas tres personas en ambas consultas**. Lo que cambió fue la justificación. En la primera respuesta señaló qué dificultad tenía cada estudiante. En la segunda relacionó esas dificultades con apoyos concretos del programa:

- **Diego** había faltado a clase para cuidar a un familiar. Las tutorías flexibles podían ayudarlo a recuperar los temas pendientes.
- **Gabriela** compartía computador en casa y tenía pocas oportunidades de practicar. Las seis horas semanales de acceso a un equipo respondían directamente a esa dificultad.
- **Ana** asistía al 95 % de las clases y estudiaba por su cuenta, pero seguía sin comprender varios conceptos básicos. Las tutorías podían ayudarla a identificar y trabajar esas dudas.

### Mi conclusión

Ana fue la única estudiante que apareció tanto en mi elección como en las dos respuestas de la IA. Yo la elegí por su constancia al asistir. La IA la eligió porque, aun con esa constancia, tenía dificultades para comprender las bases de programación.

Al comparar las respuestas, entendí que la asistencia muestra una parte del compromiso, pero por sí sola no explica qué apoyo necesita una persona. También considero importante revisar cuándo una circunstancia personal es relevante para la decisión. En el caso de Gabriela, por ejemplo, compartir computador influía directamente en su tiempo de práctica, y el programa ofrecía precisamente más horas de acceso a un equipo.

## Proyecto web · SismoTwin 4D

Dentro de la carpeta [sismTwin](./sismTwin-4d/) se encuentra mi proyecto web **SismoTwin 4D**, una página que desarrollé con apoyo de inteligencia artificial para visualizar edificios en 3D, explorar sus etapas de construcción y observar su movimiento durante una simulación sísmica.

En esa carpeta incluí dos documentos:

- **El prompt del proyecto**, donde describí lo que quería construir, cómo debía verse la página y qué funciones debía incluir.
- **El README de SismoTwin**, donde expliqué cómo funciona la página y cómo utilizar sus diferentes apartados.

**Autora:** Dahiana Diez Toro.