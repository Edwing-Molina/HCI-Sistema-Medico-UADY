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

## 4. Guion y Ejecución de Tareas

| # | Tarea para el Usuario (Script) | Escenarios Evaluados | Qué observar (Métricas Sencillas) |
| :--- | :--- | :--- | :--- |
| **1** | *"Imagine que necesita sacar una cita médica nueva. ¿Dónde presionaría para empezar?"* | Navegación Intuitiva / Reconocimiento de Acción Principal. | • ¿Duda más de 10 seg? (S/N)<br>• ¿Entró a secciones erróneas?<br>• # de clics hasta abrir el formulario. |
| **2** | *"Llene los datos de la pantalla para buscar un médico. Use el calendario para elegir el 30 de mayo."* | Flujo de Formulario / Revelación Progresiva / Selector de Fecha. | • ¿Se saltó pasos?<br>• ¿Intentó picar días grises en el calendario?<br>• ¿Preguntó cómo cambiar de mes? |
| **3** | *"En la lista de médicos, busque al Dr. Augusto Luis y elija la cita de las 10:20 AM."* | Búsqueda de Médico Específico / Precisión Motriz y Fatiga. | • ¿Notó la flecha del menú de médicos? (S/N)<br>• # de "misclicks" en las horas (píldoras).<br>• ¿Se acercó el celular a la cara para leer? |
| **4** | *"Ahora intente buscar una cita para ayer o para un domingo. ¿Qué le dice la aplicación?"* | Prevención de Citas en el Pasado / Recuperación ante Sin Resultados. | • ¿Entiende por qué no hay resultados? (S/N)<br>• ¿Se bloqueó o intentó cambiar la fecha solo? |
| **5** | *"Ya terminó su cita. Revise su lista de citas. ¿Cómo sabe que su cita se guardó bien?"* | Sensación de Logro / Orden de Lectura Lógico / Contraste en Exteriores. | • ¿Identifica el folio rápido? (S/N)<br>• ¿Sabe qué significa "Solicitada"?<br>• # de preguntas de inseguridad ("¿Ya quedó?"). |
|11|*"En su lista de citas, elija la una y busque la manera de ver toda la información detallada de esa cita en una pantalla completa.*|Consulta de Detalles / Aprendizaje / Eficiencia.|• ¿Tarda más de 5 seg en decidir picarle a la tarjeta? (S/N).• # de clics erróneos fuera de la tarjeta.• ¿Logra decirnos el campus una vez dentro del detalle?|
| **7** | *"Imagine que no es para usted, sino para su hijo/esposa. Cambie al paciente en la lista antes de buscar el médico."* | Aprendizaje / Eficiencia / Dropdowns. | • ¿Identifica el selector de "Paciente"?<br>• # de clics para abrir la lista.<br>• ¿Entiende que los datos de abajo cambian según el paciente? |
| **8** | *"Ya buscó médicos, pero ahora quiero que cambie al doctor que sale por defecto y elija a otro de la lista desplegable."* | Búsqueda de Médico Específico / Dropdowns. | • ¿Nota la flecha pequeña del menú? (S/N)<br>• ¿Logra hacer scroll dentro de la lista de nombres?<br>• # de preguntas: "¿Dónde están los otros doctores?". |
| **9** | *"Revise su lista de citas y dígame: ¿En qué Campus o Facultad le toca su consulta con el dentista?"* | Legibilidad Visual / Orden de Lectura / Contexto. | • ¿Identifica el dato del "Campus" rápidamente?<br>• ¿Confunde el campus con el nombre del médico?<br>• ¿Se acerca el celular para leer la letra pequeña? |
| **6** | *"Intente borrar la cita que acaba de hacer. Si sale un aviso, léalo en voz alta."* | Confirmación de Acción Irreversible / Legibilidad Visual (Presbicia). | • ¿Distingue el aviso rojo como advertencia?<br>• ¿Sabe cómo cerrar el aviso para NO cancelar? |
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

"¿Qué fue lo que más se le dificultó encontrar?"

"Si pudiera cambiar algo de los colores o el tamaño de los botones, ¿qué sería?"

"¿Se siente seguro de usar esto solo en su casa o pediría ayuda?"

### Criterio de Aceptación:
* **Métrica de Éxito:** El puntaje SUS debe ser **mayor a 80 puntos** para considerar el módulo de citas como satisfactorio para el personal de la UADY.