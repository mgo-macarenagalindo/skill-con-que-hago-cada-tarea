# Ejemplo de output

> Ejemplo con datos ficticios. Persona de operaciones en un negocio digital que vende un programa de formación con cuotas. Herramientas: Claude, planillas de Google, una plataforma de cursos, un CRM y Zapier. Dos tareas manejan datos de alumnos.

# Con qué hago cada tarea · semana del 16 de noviembre

## Tabla de decisión
| Tarea | Veces/semana · minutos | Salida | Por qué (una línea) | Herramienta |
|---|---|---|---|---|
| Mandar al equipo de ventas el mensaje diario con las agendas del día | 5 · 10 (50/sem) | 1 · Eliminar | El CRM ya muestra las agendas en una vista; el mensaje repite lo mismo | Ninguna: una vista guardada en el CRM |
| Aprobar excepciones de cuotas que piden los alumnos | 3 · 20 (60/sem) | 2 · Delegar | Es una decisión comercial: le corresponde al closer, con un tope escrito | Proceso escrito de una página |
| Decidir qué hacer con cada pago rechazado (reintentar, avisar, pausar el acceso) | 6 · 10 (60/sem) | 3 · La hacés vos y la documentás | Hoy cada caso se resuelve distinto; sin criterio escrito, ninguna herramienta lo puede hacer bien | Un documento con los casos y qué se hace en cada uno |
| Pasar cada alumno nuevo de la pasarela a la planilla de alumnos | 15 · 4 (60/sem) | 4 · Automatizar | Es copiar los mismos campos, siempre igual | Zapier: pago aprobado → fila nueva en la planilla |
| Responder en la comunidad las preguntas frecuentes de alumnos | 20 · 5 (100/sem) | 5 · IA en un chat | Termina en un texto y las respuestas ya existen en las clases | Claude, con un pedido fijo y la lista de respuestas aprobadas |
| Resumir la reunión semanal de equipo y repartir pendientes | 1 · 40 (40/sem) | 5 · IA en un chat | Es resumir una transcripción que ya tenés | Claude |
| Conciliar los cobros de la pasarela con la planilla de cuotas | 1 · 120 (120/sem) [ESTIMADO] | 5 · IA en un chat | Es comparar dos exports y marcar diferencias | Claude, con los dos exports sin nombres ni mails |
| Dar de alta a cada alumno nuevo en la plataforma de cursos | 15 · 3 (45/sem) | 6 · IA que trabaja en el navegador | Son clics en una web que no tiene integración con la pasarela | IA en el navegador, o pasos escritos y los clics los hacés vos |
| Armar el reporte semanal de ventas para el founder | 1 · 60 (60/sem) | 7 · Skill o agente | Ya lo hacés con IA en un chat hace un mes, siempre con el mismo export y el mismo formato | Una skill que arma el reporte siempre igual |

## Pedidos listos para pegar (solo las tareas que van a IA)

**Preguntas frecuentes de la comunidad**
> **Contexto:** soy de operaciones en un programa de formación. Los alumnos preguntan en la comunidad cosas que ya están respondidas en las clases. **Objetivo:** redactá una respuesta corta y cordial a la pregunta que te pego, usando solo las respuestas aprobadas. **Fuente:** la lista de respuestas aprobadas [completar: pegar la lista] y la pregunta, sin el nombre del alumno. **Formato:** tres a cinco líneas, con voseo, y al final el nombre de la clase donde está la respuesta. Si la pregunta no está en la lista, decime «no está en las respuestas aprobadas» y no inventes.

**Resumen de la reunión semanal**
> **Contexto:** reunión semanal del equipo de operaciones y ventas. **Objetivo:** que cada persona sepa qué tiene que hacer esta semana. **Fuente:** la transcripción que te pego. **Formato:** decisiones tomadas (una línea cada una), pendientes en tabla (pendiente · responsable · fecha) y temas que quedaron abiertos. Si un pendiente no tiene responsable, marcalo [completar].

**Conciliación de cobros**
> **Contexto:** cobramos cuotas por una pasarela y las registramos en una planilla. **Objetivo:** encontrar diferencias entre lo que dice la planilla y lo que dice la pasarela. **Fuente:** dos exports de la semana, solo con ID de venta, fecha, monto y estado [completar: pegar los dos]. **Formato:** tabla con ID · monto en planilla · monto en pasarela · diferencia · qué revisar. Lo que coincide no lo muestres.

**Alta en la plataforma de cursos (IA en el navegador)**
> **Contexto:** cada alumno nuevo tiene que quedar dado de alta en la plataforma de cursos con su programa. **Objetivo:** dar de alta a los alumnos de la lista y avisarme si alguno ya existía. **Fuente:** la lista de alumnos nuevos de la semana [completar]. **Formato:** al terminar, una tabla con alumno · alta hecha / ya existía / error. No cambies nada que no sea dar de alta.

## Tu experimento de estas dos semanas
| Tarea | Línea de base | Qué probás | Qué medís | Fecha de decisión |
|---|---|---|---|---|
| Mensaje diario de agendas | 50 min por semana · 0 errores | Dejás de mandarlo y el equipo de ventas usa la vista del CRM | Minutos que liberás y cuántas veces alguien pregunta por una agenda | Viernes 4 de diciembre |

Es la tarea con más minutos entre las de salida más simple: eliminar no necesita ninguna herramienta nueva. Si en dos semanas nadie pregunta por las agendas, queda eliminada y pasás a las preguntas frecuentes de la comunidad, que es la que más tiempo te lleva. Si preguntan seguido, volvés a mandarlo y probás la siguiente salida de la tabla.

## Lo que no conviene tocar todavía (y por qué)
- **Pagos rechazados:** primero hay que escribir qué se hace en cada caso. Automatizar un criterio que no existe es automatizar el desorden.
- **Excepciones de cuotas:** no van a la IA. Es una decisión comercial y tiene que tener dueño.
- **Reporte semanal como skill:** espera a que termine el experimento. Una tarea por vez.

---

**Horas que se podrían liberar si todo funcionara:** unas 5,5 horas por semana (330 de los 475 minutos de las tareas con tiempo real). Lo eliminado y lo delegado se libera entero; en las que pasan a IA o a automatización queda tiempo de revisión; los pagos rechazados no liberan tiempo todavía, porque primero los documentás vos. La conciliación de cobros, que está estimada en 2 horas, liberaría cerca de 1 hora más; confirmá cuánto te lleva antes de contarla.

Una tarea por vez: la próxima se elige cuando esta tenga su número.
