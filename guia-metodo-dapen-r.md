# Método DAPEN+R: guía para escribir buenos prompts

## ¿Qué es?

El **Método DAPEN+R** es una forma sencilla de escribir **prompts**, es decir, las instrucciones que damos a una IA como ChatGPT, Claude, Gemini o Copilot. Fue creado por **Daniel Peña**, de DAPEN Centro de Estudios.

Funciona como una **lista de comprobación**: siete preguntas que respondes antes de escribir. La idea clave es esta:

> **La IA no adivina lo que piensas. Solo trabaja con lo que le escribes.**

## Los siete componentes

| Componente | Pregunta | Qué escribes | Ejemplo |
|---|---|---|---|
| **Rol** | ¿Qué papel debe adoptar la IA? | La profesión o experiencia desde la que responde. | «Eres un responsable de administración.» |
| **Acción** | ¿Qué tiene que hacer exactamente? | Un verbo claro: redacta, resume, explica, compara, crea. | «Redacta un correo para recordar el pago de una factura.» |
| **Datos** | ¿Con qué información trabaja? | Los datos concretos: nombres, cifras, fechas o el texto a trabajar. | «Factura 2026-045, 350 €, venció el 15 de octubre.» |
| **Público** | ¿A quién va dirigido? | Quién lo va a leer o escuchar. | «La persona de contabilidad del cliente.» |
| **Estilo** | ¿Con qué tono y formato? | El tono, el formato y la extensión. | «Amable y firme. Trato de usted. Máximo 100 palabras.» |
| **Negación** | ¿Qué debe evitar? | Lo que no quieres que aparezca, mejor con el motivo. | «Sin amenazas, porque queremos conservar al cliente.» |
| **Revisión** | ¿Qué debe comprobar antes de entregarlo? | Una comprobación final y qué hacer si falta algo. | «Comprueba que aparecen la factura y el importe. Si falta un dato, dímelo.» |

**El nombre:** **DAPEN** recoge cinco componentes (**D**atos, **A**cción, **P**úblico, **E**stilo y **N**egación). La **+R** añade las dos **R**: **R**ol, que abre el prompt, y **R**evisión, que lo cierra.

## Cómo usarlo en tres pasos

1. **Piensa.** Responde mentalmente a las siete preguntas.
2. **Escribe.** Una línea por componente, en este orden.
3. **Lee y ajusta.** Revisa el resultado y pide los cambios que necesites.

## Recuerda

- **No pegues datos personales ni confidenciales** en una IA.
- Los resultados **pueden variar**: lee siempre el texto antes de usarlo.
- Si no sale como esperabas, **mejora el prompt y vuelve a probar**.

## Tres ejemplos reales

*Todos los datos son ficticios.*

### Ejemplo 1. En el correo: recordar el pago de una factura

```text
Rol: Eres un responsable de administración.
Acción: Redacta un correo para recordar el pago de una factura.
Datos: Factura 2026-045, 350 €, venció el 15 de octubre. Es el primer aviso.
Público: La persona de contabilidad del cliente.
Estilo: Amable y firme. Trato de usted. Máximo 100 palabras.
Negación: Sin amenazas ni reproches, porque queremos conservar al cliente.
Revisión: Antes de entregarlo, comprueba que aparecen la factura, el importe y la fecha.
```

*Fíjate en los **Datos**: con cifras y fechas concretas, la IA no tiene que inventar nada.*

### Ejemplo 2. En el aula: crear un ejercicio de Word

```text
Rol: Eres un profesor de ofimática con experiencia en formación para adultos.
Acción: Crea un ejercicio práctico de Word de 20 minutos.
Datos: Tema: dar formato a una carta comercial (tipo de letra, márgenes, tabla de precios y pie de página).
Público: Alumnos adultos de un curso de ofimática básica.
Estilo: Pasos numerados, lenguaje sencillo, máximo una página.
Negación: Explica cada paso con palabras sencillas, sin tecnicismos, porque nunca han usado Word.
Revisión: Comprueba que el ejercicio se puede hacer en 20 minutos y que indica el resultado esperado.
```

*Fíjate en el **Público**: decir quién lo va a usar cambia el nivel y el lenguaje.*

### Ejemplo 3. En la empresa: resumir las ventas para la dirección

```text
Rol: Eres un analista comercial.
Acción: Redacta un resumen de las ventas del trimestre para la dirección.
Datos: Ventas del tercer trimestre: 120.000 €. Ventas del segundo trimestre: 100.000 €. Producto más vendido: formación presencial.
Público: La dirección, que solo tiene dos minutos para leerlo.
Estilo: Tres frases, tono profesional, indicando la subida en porcentaje.
Negación: No añadas datos que no aparezcan arriba, porque la dirección tomará decisiones con este resumen.
Revisión: Comprueba el cálculo del porcentaje y muéstrame la operación.
```

*Fíjate en la **Revisión**: pedir la operación te permite comprobar el cálculo tú mismo.*

## Tu plantilla

Copia estas líneas y rellénalas:

```text
Rol:
Acción:
Datos:
Público:
Estilo:
Negación:
Revisión:
```

## Texto del método para pegar en Claude

Cópialo y pégalo en las preferencias de tu cuenta, en las instrucciones de un proyecto o al inicio de una conversación. Así Claude conocerá el método.

```text
MÉTODO DAPEN+R (versión oficial 2.0, noviembre de 2026)

El Método DAPEN+R es un método para redactar prompts creado por Daniel Peña, de DAPEN Centro de Estudios (Valencia). Se compone de siete componentes, que se escriben en este orden, uno por línea:

1. Rol: ¿qué papel debe adoptar la IA?
2. Acción: ¿qué tiene que hacer exactamente?
3. Datos: ¿con qué información trabaja?
4. Público: ¿a quién va dirigido el resultado?
5. Estilo: ¿con qué tono y formato?
6. Negación: ¿qué debe evitar?
7. Revisión: ¿qué debe comprobar antes de entregarlo?

Significado del nombre: DAPEN recoge cinco componentes (Datos, Acción, Público, Estilo y Negación). La +R añade las dos R: Rol, que abre el prompt, y Revisión, que lo cierra.

Cuando te pida ayuda con un prompt:
- Usa estos siete componentes y este orden. No propongas otras versiones ni otros significados del nombre.
- Si falta información en algún componente, pregúntame antes de redactarlo en lugar de suponerla.
- Escribe en español de España.
```

*Las tres últimas líneas son opcionales: si solo quieres que Claude conozca el método, bórralas.*

*Método DAPEN+R · Versión 2.0 · Noviembre de 2026 · DAPEN Centro de Estudios · www.dapencentroestudios.com*
