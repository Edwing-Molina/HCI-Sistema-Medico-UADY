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
| **1** | *"Observe la pantalla. Sin tocar nada todavía, ¿le parece que este es un sitio seguro de la UADY? ¿Dónde picaría para entrar?"* | Confianza / Reconocimiento de Flujo. | • ¿Identifica el logo institucional? (S/N)<br>• ¿Ubica el botón de Login rápido?<br>• ¿Duda de si es la app oficial? |
| **2** | *"Escriba su correo, pero olvide poner el '@' o el '.mx' adrede. Luego intente entrar."* | Validación de Formato de Email. | • ¿Aparece el mensaje de error de inmediato?<br>• ¿Entiende que el error es el correo y no la clave?<br>• ¿Lo corrige sin ayuda? |
| **3** | *"Ahora borre todo e intente darle al botón de 'Entrar' con los cuadritos vacíos."* | Envío de Campos Vacíos. | • ¿El sistema bloquea el botón o marca error?<br>• ¿Entiende qué campo le falta llenar?<br>• # de clics extra al botón vacío. |
| **4** | *"Ponga su correo bien, pero escriba una contraseña que NO sea la suya e intente entrar."* | Error de Credenciales. | • ¿El mensaje de error es claro? (S/N)<br>• ¿Identifica el icono de error (sin depender del color rojo)?<br>• # de intentos antes de pedir ayuda. |
| **6** | *"Escriba su clave real y, en lugar de picar el botón dorado, use la tecla 'Entrar' (Enter) de su teclado de pantalla."* | Navegación con Teclado. | • ¿Inicia sesión al picar 'Enter'? (S/N)<br>• ¿Se queda esperando a que pase algo?<br>• ¿Duda de si el teclado sirve para entrar? |
| **7** | *"Mientras el sistema carga, dígame: ¿La app le está avisando que está trabajando o parece que se trabó?"* | Visibilidad del Estado de Carga. | • ¿Nota el indicador de carga (spinner)?<br>• ¿Intenta picar el botón muchas veces mientras carga?<br>• ¿Reconoce que el botón se desactivó? |
| **8** | *"Cierre la aplicación por completo y vuélvala a abrir. ¿Le volvió a pedir su clave o lo dejó entrar directo?"* | Persistencia de Sesión (Satisfacción). | • ¿Entró directo a la pantalla principal? (S/N)<br>• ¿Se ve aliviado de no tener que escribir todo otra vez? |        
|**5** |<mark> Pendiente a revsion </mark> *"Imagine que no trae sus lentes. Vamos a hacer la letra más grande (200%). ¿Puede seguir leyendo todo bien o se amontonó la letra?"* | Escalado de Interfaz (Accesibilidad). | • ¿Se enciman los textos o botones? (S/N)<br>• ¿Aparece barra de desplazamiento (scroll)?<br>• ¿Puede leer las etiquetas de los campos? |

###  Guion y Ejecución de Tareas (Citas)

| # | Tarea para el Usuario (Script) | Escenarios Evaluados | Qué observar (Métricas Sencillas) |
| :--- | :--- | :--- | :--- |
| **1** | *"Imagine que necesita sacar una cita médica nueva. ¿Dónde presionaría para empezar?"* | Navegación Intuitiva / Reconocimiento de Acción Principal. | • ¿Duda más de 10 seg? (S/N)<br>• ¿Entró a secciones erróneas?<br>• # de clics hasta abrir el formulario. |
| **2** | *"Llene los datos de la pantalla para buscar un médico. Use el calendario para elegir el 30 de mayo."* | Flujo de Formulario / Revelación Progresiva / Selector de Fecha. | • ¿Se saltó pasos?<br>• ¿Intentó picar días grises en el calendario?<br>• ¿Preguntó cómo cambiar de mes? |
| **3** | *"En la lista de médicos, busque al Dr. Augusto Luis y elija la cita de las 10:20 AM."* | Búsqueda de Médico Específico / Precisión Motriz y Fatiga. | • ¿Notó la flecha del menú de médicos? (S/N)<br>• # de "misclicks" en las horas (píldoras).<br>• ¿Se acercó el celular a la cara para leer? |
| **4** | *"Ahora intente buscar una cita para ayer o para un domingo. ¿Qué le dice la aplicación?"* | Prevención de Citas en el Pasado / Recuperación ante Sin Resultados. | • ¿Entiende por qué no hay resultados? (S/N)<br>• ¿Se bloqueó o intentó cambiar la fecha solo? |
| **5** | *"Ya terminó su cita. Revise su lista de citas. ¿Cómo sabe que su cita se guardó bien?"* | Sensación de Logro / Orden de Lectura Lógico / Contraste en Exteriores. | • ¿Identifica el folio rápido? (S/N)<br>• ¿Sabe qué significa "Solicitada"?<br>• # de preguntas de inseguridad ("¿Ya quedó?"). |
|**6**|*"En su lista de citas, elija la una y busque la manera de ver toda la información detallada de esa cita en una pantalla completa.*|Consulta de Detalles / Aprendizaje / Eficiencia.|• ¿Tarda más de 5 seg en decidir picarle a la tarjeta? (S/N).• # de clics erróneos fuera de la tarjeta.• ¿Logra decirnos el campus una vez dentro del detalle?|
| **7** | *"Imagine que no es para usted, sino para su hijo/esposa. Cambie al paciente en la lista antes de buscar el médico."* | Aprendizaje / Eficiencia / Dropdowns. | • ¿Identifica el selector de "Paciente"?<br>• # de clics para abrir la lista.<br>• ¿Entiende que los datos de abajo cambian según el paciente? |
| **8** | *"Ya buscó médicos, pero ahora quiero que cambie al doctor que sale por defecto y elija a otro de la lista desplegable."* | Búsqueda de Médico Específico / Dropdowns. | • ¿Nota la flecha pequeña del menú? (S/N)<br>• ¿Logra hacer scroll dentro de la lista de nombres?<br>• # de preguntas: "¿Dónde están los otros doctores?". |
| **9** | *"Revise su lista de citas y dígame: ¿Que datos puede ver de su cita?"* | Legibilidad Visual / Orden de Lectura / Contexto. | • ¿Identifica los datos de su cita?<br>•<br>• ¿Se acerca el celular para leer la letra pequeña? |
| **10** | *"Intente borrar la cita que acaba de hacer. Si sale un aviso, léalo en voz alta."* | Confirmación de Acción Irreversible / Legibilidad Visual (Presbicia). | • ¿Distingue el aviso rojo como advertencia?<br>• ¿Sabe cómo cerrar el aviso para NO cancelar? |
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

"¿Qué prefiere: que la app se acuerde de usted (Sesión persistente) o poner la clave siempre por seguridad?"

"¿Qué fue lo que más se le dificultó encontrar?"

"Si pudiera cambiar algo de los colores o el tamaño de los botones, ¿qué sería?"

"¿Se siente seguro de usar esto solo en su casa o pediría ayuda?"

### Criterio de Aceptación:
* **Métrica de Éxito:** El puntaje SUS debe ser **mayor a 80 puntos** para considerar el módulo de citas como satisfactorio para el personal de la UADY.





