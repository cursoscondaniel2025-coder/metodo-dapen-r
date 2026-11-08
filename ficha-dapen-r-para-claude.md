# Ficha didáctica: DAPEN+R para Claude

**Cuatro mejoras para obtener mejores respuestas, sin cambiar el método.**

## 1. Título y datos

| | |
|---|---|
| **Tema** | Cómo aplicar el Método DAPEN+R con Claude |
| **Nivel** | Intermedio (con un repaso inicial del método) |
| **Duración estimada** | 60 minutos |
| **Herramienta** | Claude |
| **Versión** | 1.1 · noviembre de 2026 |

> **Importante:** esta ficha no modifica el Método DAPEN+R. Los siete componentes son los mismos. Aquí se recogen consejos complementarios, basados en la guía de buenas prácticas de Anthropic, que ayudan a obtener mejores resultados con Claude.

## 2. Repaso previo: el Método DAPEN+R

El Método DAPEN+R, creado por Daniel Peña, es una forma sencilla de no olvidar nada al escribir un prompt. Tiene siete componentes y cada uno responde a una pregunta.

| Componente | Pregunta guía | Ejemplo |
|---|---|---|
| **Rol** | ¿Qué papel debe adoptar la IA? | Eres un responsable de administración. |
| **Acción** | ¿Qué tiene que hacer exactamente? | Escribe un correo para recordar el pago de una factura. |
| **Datos** | ¿Con qué información trabaja? | Factura 2026-045, 350 €, venció el 15 de octubre. |
| **Público** | ¿A quién va dirigido el resultado? | La persona de contabilidad del cliente. |
| **Estilo** | ¿Con qué tono y formato? | Amable y firme. Trato de usted. Máximo 100 palabras. |
| **Negación** | ¿Qué debe evitar? | Sin amenazas ni reproches. |
| **Revisión** | ¿Qué debe comprobar antes de entregarlo? | Que aparecen la factura, el importe y la fecha. |

**El nombre:** DAPEN recoge cinco componentes (Datos, Acción, Público, Estilo y Negación) y la +R añade las dos R: Rol, que abre el prompt, y Revisión, que lo cierra.

> A lo largo de la ficha usaremos **siempre el mismo caso**: un correo para recordar a un cliente el pago de una factura.

## 3. Objetivos de aprendizaje

Al terminar la sesión, el alumnado será capaz de:

- Identificar qué información falta en un prompt DAPEN+R.
- Aplicar ejemplos y formulaciones en positivo para mejorar un prompt.
- Reescribir un prompt de uso real incorporando los cuatro consejos.
- Comprobar el resultado antes y después de recibirlo.

## 4. Conceptos clave

### Concepto 1. Cuenta el para qué

Claude responde mejor cuando sabe **para qué** quieres el texto, no solo qué texto quieres.

**Dónde encaja:** Acción.

- ❌ **Antes:** «Escribe un correo para recordar el pago de una factura.»
- ✅ **Después:** «Escribe un correo para recordar el pago de una factura. Queremos cobrar esta semana sin molestar al cliente, que siempre paga a tiempo.»

### Concepto 2. Enséñale con un ejemplo

Un ejemplo de lo que quieres vale más que muchas explicaciones. La guía de Anthropic recomienda de 3 a 5 ejemplos variados; con uno solo, Claude puede copiarlo demasiado.

**Dónde encaja:** Estilo.

- ❌ **Antes:** «Escribe un correo amable.»
- ✅ **Después:** «Escribe un correo con este estilo: *Hola, Marta: te escribo para recordarte la factura 2026-040. Seguro que se te ha pasado. ¿Puedes confirmarme el pago esta semana? Gracias.*»

### Concepto 3. Pide lo que quieres, y explica el motivo

Funciona mejor decir **qué quieres** que decir qué no quieres. Añade el porqué y la extensión.

**Dónde encaja:** Negación y Estilo.

- ❌ **Antes:** «No seas agresivo.»
- ✅ **Después:** «Usa un tono amable, porque queremos seguir trabajando con este cliente. Máximo 100 palabras.»

### Concepto 4. Ordena la información y revisa dos veces

**Ordena.** Si el prompt es largo, separa cada parte con un título o una etiqueta. Las etiquetas funcionan como cajones: cada información va en el suyo.

```text
<datos>Factura 2026-045, 350 €, venció el 15 de octubre.</datos>
<ejemplo>Hola, Marta: te escribo para recordarte la factura 2026-040...</ejemplo>
```

En un prompt corto no hacen falta.

**Revisa dos veces.** La Revisión tiene dos momentos:

- **Antes de entregar:** Claude comprueba lo que le pides. Por ejemplo: «Antes de entregarlo, comprueba que aparecen la factura y el importe. Si falta algún dato, dímelo.»
- **Después de entregar:** lees tú el resultado. Ninguna comprobación de Claude sustituye tu lectura.

**Dónde encaja:** Datos y Revisión.

## 5. Actividad práctica: mejora tu prompt en 4 pasos

**Duración:** 25 minutos, en parejas. Usa siempre datos ficticios.

**Punto de partida:**

```text
Rol: Eres un responsable de administración.
Acción: Escribe un correo para recordar el pago de una factura.
Datos: Factura 2026-045, 350 €, venció el 15 de octubre. Es el primer aviso.
Público: La persona de contabilidad del cliente.
Estilo: Amable y firme. Trato de usted. Máximo 100 palabras.
Negación: Sin amenazas ni reproches.
Revisión: Antes de entregarlo, comprueba que aparecen la factura, el importe y la fecha.
```

**Pasos:**

1. **Añade el para qué** a la Acción: «Queremos cobrar esta semana sin molestar al cliente, que siempre paga a tiempo.»
2. **Añade un ejemplo** al Estilo: «Sigue este ejemplo: Hola, Marta: te escribo para recordarte la factura 2026-040. Seguro que se te ha pasado. ¿Puedes confirmarme el pago esta semana? Gracias.»
3. **Reescribe la Negación** pidiendo lo que quieres y con el motivo: «Usa un tono amable, porque queremos seguir trabajando con este cliente.»
4. **Pide que avise si falta algo:** «No inventes datos: si falta alguno, dímelo.»
5. **Prueba:** ejecuta el prompt de partida y el mejorado, tres veces cada uno, y anota cuántas correcciones necesita cada resultado. Enseña también el prompt a un compañero sin contexto: si a él le confunde, a Claude también.

**Resultado esperado:** un prompt como este.

```text
Rol: Eres un responsable de administración.
Acción: Escribe un correo para recordar el pago de una factura. Queremos cobrar esta semana sin molestar al cliente, que siempre paga a tiempo.
Datos: Factura 2026-045, 350 €, venció el 15 de octubre. Es el primer aviso.
Público: La persona de contabilidad del cliente. Recibe muchos correos.
Estilo: Amable y firme. Trato de usted. Máximo 100 palabras. Sigue este ejemplo: «Hola, Marta: te escribo para recordarte la factura 2026-040. Seguro que se te ha pasado. ¿Puedes confirmarme el pago esta semana? Gracias.»
Negación: Usa un tono amable, porque queremos seguir trabajando con este cliente. No inventes datos: si falta alguno, dímelo.
Revisión: Antes de entregarlo, comprueba que aparecen la factura, el importe y la fecha.
```

Los resultados de la IA pueden variar entre ejecuciones. Por eso se repite la prueba varias veces antes de sacar conclusiones.

## 6. Resumen

- Los siete componentes de DAPEN+R no cambian; estos consejos son un complemento opcional para Claude.
- Cuenta el para qué: Claude se adapta mejor.
- Enseña con un ejemplo y pide lo que quieres, con el motivo.
- Ordena con etiquetas si el prompt es largo, y revisa antes y después de recibir el resultado.

## 7. Comprobación rápida

1. ¿Por qué conviene añadir el para qué en la Acción?
   *(Porque, si Claude entiende el objetivo, puede adaptarse a situaciones que las instrucciones no han previsto.)*
2. Reescribe pidiendo lo que quieres y con motivo: «No uses un tono agresivo con el cliente.»
   *(Por ejemplo: «Usa un tono amable, porque queremos seguir trabajando con este cliente.»)*

## Fuentes y verificación

Consejos basados en la guía de buenas prácticas de prompts de Anthropic, consultada en noviembre de 2026 (docs.claude.com, sección *Prompt engineering*). La correspondencia de cada consejo con los componentes de DAPEN+R es una propuesta de adaptación. Los modelos y su comportamiento cambian con frecuencia: conviene revisar la documentación oficial antes de enseñar esta ficha.

*Método DAPEN+R · Autor: Daniel Peña · DAPEN Centro de Estudios.*
