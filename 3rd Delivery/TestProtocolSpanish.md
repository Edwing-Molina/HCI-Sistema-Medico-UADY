# Protocolo de Pruebas: Módulo de Citas (Servicio Médico UADY)

## 1. Perfil de los Participantes
* **Población:** Personal de mantenimiento, limpieza y administrativos de la UADY.
* **Rango de edad:** 45 a 55 años.
* **Nivel digital:** Bajo (no conocen el sistema).
* **Condición física:** Posible fatiga motriz (tras jornada laboral) y fatiga visual.

## 2. Instrucciones para el Moderador
1.  **Neutralidad:** No ayude al usuario. Si se queda bloqueado, pregunte: *"¿Qué cree que debería pasar aquí?"*.
2.  **Pensar en voz alta:** Pida al usuario que narre lo que está viendo y por qué toma cada decisión.
3.  **Entorno:** Realizar la prueba en un lugar con luz natural para validar el contraste y visibilidad.

## 3. Guion de Bienvenida (Empatía)
"Hola, muchas gracias por ayudarnos. Estamos probando una nueva aplicación para las citas médicas de la UADY. No lo estamos evaluando a usted, estamos evaluando a la aplicación. Si algo no sale bien o no encuentra una opción, no es culpa suya, es que nosotros debemos mejorar el diseño. Por favor, trate de decir en voz alta todo lo que vaya pensando o lo que le confunda."

---
## Guione y Tareas

###  Guion y Ejecución de Tareas (Login)

| # | Tarea para el Usuario (Script) | Escenarios Evaluados | Qué observar (Métricas Sencillas) |
| :--- | :--- | :--- | :--- |
| **1** | *"Entre en la aplicacion y intente iniciar sesion con sus credenciales"* | Confianza / Reconocimiento de Flujo. | • ¿Ubica el botón de Login rápido? |
| **** | *"II"* | Validación de Formato de Email. | • ¿Entiende que el error es el correo y no la clave?<br>• ¿Lo corrige sin ayuda? |
| **** | *"II"* | Envío de Campos Vacíos. | • ¿Entiende qué campo le falta llenar?<br>• # de clics extra al botón vacío. |
| **** | *"II"* | Error de Credenciales. | • # de intentos antes de pedir ayuda. |
| **** | *"II"* | Visibilidad del Estado de Carga. | • ¿Nota el indicador de carga (spinner)?<br>• ¿Intenta picar el botón muchas veces mientras carga?<br> |
| **2** | *"Cierre la aplicación por completo y vuélvala a abrir."* | Persistencia de Sesión (Satisfacción). | • ¿Entró directo a la pantalla principal? (S/N)<br>•  |        

###  Guion y Ejecución de Tareas (Citas)

| # | Tarea para el Usuario (Script) | Escenarios Evaluados | Qué observar (Métricas Sencillas) |
| :--- | :--- | :--- | :--- |
| **1** | *"Agende una cita medica para la especialidad de medicina general en el turno matutino para el dia 29 de mayo de 2026 con el doctor JOSE ROBERTO HERRERA GAMBOA a las 11:40"* | Navegación Intuitiva / Reconocimiento de Acción Principal. | • ¿Entró a secciones erróneas?<br>• # de clics hasta abrir el formulario. |
|  | *"II"* | Flujo de Formulario / Revelación Progresiva / Selector de Fecha. | • ¿Se saltó pasos?<br>• ¿Intentó picar días grises en el calendario?<br>• ¿Preguntó cómo cambiar de mes? |
|  | *"II"* | Búsqueda de Médico Específico / Precisión Motriz y Fatiga. | • ¿Notó la flecha del menú de médicos? (S/N)<br>• # de "misclicks" en las horas (píldoras).<br>• ¿Se acercó el celular a la cara para leer? |
|  | *"II"* | Búsqueda de Médico Específico / Dropdowns. | • ¿Nota la flecha pequeña del menú? (S/N)<br>• ¿Logra hacer scroll dentro de la lista de nombres?<br>• # de preguntas: "¿Dónde están los otros doctores?". |
| **2** | *"Ya terminó su cita. Revise su lista de citas. Y digame como sabe que su cita se realizo correctamente"* | Sensación de Logro / Orden de Lectura Lógico / Contraste en Exteriores. | • ¿Identifica el folio rápido? (S/N)<br>• ¿Sabe qué significa "Solicitada"?<br>• # de preguntas de inseguridad ("¿Ya quedó?"). |
| **3** | *"Revise su lista de citas y dígame: ¿Que datos puede ver de su cita?"* | Legibilidad Visual / Orden de Lectura / Contexto. | • ¿Identifica los datos de su cita?<br>• ¿Se acerca el celular para leer la letra pequeña? |
|**4**|*"En su lista de citas,busque la manera de ver toda la información detallada de la cita que acaba de agendar. Y diganos toda la informacion de la cita*|Consulta de Detalles / Aprendizaje / Eficiencia.|• # de clics erróneos fuera de la tarjeta.• ¿Logra decirnos la informacion una vez dentro del detalle?|
| **5** | *"Ahora intente agendar una cita para el dia 29 de abril en la especialidad de medicina general para el turno matutino y digame si le permite hacer la cita o lo que sucede"* | Prevención de Citas en el Pasado / Recuperación ante Sin Resultados. | • ¿Entiende por qué no hay resultados? (S/N)<br>• ¿Se bloqueó o intentó cambiar la fecha solo? |
| **6** | *"Intente agendar una cita para cualquier beneficiario que tenga, para medicina general para el dia 27 de mayo turno matutino con el medico OSCAR FUENTES LUGO"* | Aprendizaje / Eficiencia / Dropdowns. | • ¿Identifica el selector de "Paciente"?<br>• # de clics para abrir la lista.<br>• ¿Desde donde hace elige al beneficiario?¿Desde el home de citas o desde el agendado de citas? |
| **7** | *"Cancele las dos citas que acaba de hacer. Si sale un aviso, léalo en voz alta, y digame cuantas cancelaciones le quedan"* | Confirmación de Acción Irreversible / Legibilidad Visual (Presbicia). | • ¿Logra cancelar las citas?<br>• ¿Sabe cuantas cancelaciones le quedan? ¿Pregunta sobre las opciones en el modal de cancelacion? |
---

## 5. Hoja de Registro de Métricas (Para el Evaluador)

Use esta tabla para anotar los resultados de cada participante de forma rápida:

| Participante | Tarea # | ¿Terminó la tarea? | # de Clics | # de Preguntas/Dudas | # de Errores/Tropiezos |
| :--- | :---: | :---: | :---: | :---: | :---: |
| | 1 | [ ] Sí [ ] No | | | |
| | 2 | [ ] Sí [ ] No | | | |
| | 3 | [ ] Sí [ ] No | | | |
| | 4 | [ ] Sí [ ] No | | | |
| | 5 | [ ] Sí [ ] No | | | |
| | 6 | [ ] Sí [ ] No | | | |
| | 7 | [ ] Sí [ ] No | | | |
| | 8 | [ ] Sí [ ] No | | | |

---

## 6. Cierre y Evaluación de Satisfacción (SUS)

Al finalizar las tareas, entregue al usuario el formato **SUS (System Usability Scale)** simplificado. Como los usuarios son de perfil operativo, puede leerles las preguntas y marcar sus respuestas en la escala del 1 al 5:

1.  Creo que usaría esta aplicación con frecuencia.
2.  Encontré la aplicación innecesariamente compleja.
3.  Pensé que la aplicación era fácil de usar.
4.  Creo que necesitaría el apoyo de un técnico para poder usar esta aplicación.
5.  Encontré que las diversas funciones de la aplicación estaban bien integradas.
6.  Pensé que había demasiada inconsistencia en esta aplicación.
7.  Imagino que la mayoría de la gente aprendería a usar esta aplicación muy rápidamente.
8.  Encontré la aplicación muy pesada de usar.
9.  Me sentí muy seguro usando la aplicación.
10. Necesité aprender muchas cosas antes de poder seguir con la aplicación.

### Cierre Cualitativo (Post-Test)
Después del SUS, haz estas 3 preguntas abiertas. A veces valen más que cualquier métrica:

"¿Qué prefiere: que la app se acuerde de usted (Sesión persistente) o poner la clave siempre por seguridad?"

"¿Qué fue lo que más se le dificultó encontrar?"

"Si pudiera cambiar algo de los colores o el tamaño de los botones, ¿qué sería?"

"¿Se siente seguro de usar esto solo en su casa o pediría ayuda?"

### Criterio de Aceptación:
* **Métrica de Éxito:** El puntaje SUS debe ser **mayor a 80 puntos** para considerar el módulo de citas como satisfactorio para el personal de la UADY.





