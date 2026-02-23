# Especificación de Requisitos - App Servicio Médico UADY

Este documento detalla los requisitos funcionales y no funcionales para la aplicación destinada a los derechohabientes del servicio médico de la Universidad Autónoma de Yucatán.

## 1. Requisitos Funcionales (RF)

| ID | Nombre del Requisito | Descripción |
| :--- | :--- | :--- |
| **RF01** | **Pantalla de Bienvenida** | El sistema debe mostrar una pantalla de inicio con los colores institucionales y la versión de la app durante un mínimo de 1.5 segundos como indicador de carga visual. |
| **RF02** | **Autenticación Office 365** | El sistema debe permitir el inicio de sesión mediante una cuenta institucional de Office 365 a través de un botón dedicado. |
| **RF03** | **Validación de Vigencia** | Al iniciar sesión, el sistema debe verificar en tiempo real si el empleado está vigente en la base de datos; de lo contrario, mostrar el mensaje: "El usuario no está vigente". |
| **RF04** | **Persistencia de Datos** | El sistema debe almacenar en el local storage el token de acceso, nombre completo, correo electrónico y clave del empleado para evitar consultas redundantes. |
| **RF05** | **Cierre de Sesión Seguro** | La app debe invalidar los tokens de Office 365 y de la API local, presentando un modal de confirmación antes de proceder. |
| **RF06** | **Selección de Paciente** | El sistema debe permitir elegir entre el empleado o sus derechohabientes mediante un selector obligatorio que actualice la interfaz dinámicamente. |
| **RF07** | **Agendado de Citas** | El usuario podrá seleccionar especialidad, turno, fecha y médico. El calendario se habilitará solo tras seleccionar especialidad y turno. |
| **RF08** | **Visualización por Campus** | El sistema debe filtrar médicos y horarios disponibles basándose en el campus de adscripción del empleado (ej. Ciencias Exactas, Sociales). |
| **RF09** | **Listado y Detalle** | Mostrar citas futuras en orden cronológico con detalle completo: folio, médico, especialidad, turno, fecha y hora (formato 24h). |
| **RF10** | **Cancelación de Citas** | Permitir cancelar citas desde el listado/detalle con un modal que advierta: "Esta cancelación cuenta para tu límite anual". |
| **RF11** | **Límite de Cancelaciones** | El sistema debe bloquear el agendado automáticamente al alcanzar el límite configurable (por defecto 3 cancelaciones). |
| **RF12** | **Bloqueo Administrativo** | Si el usuario está bloqueado, mostrar un mensaje persistente indicando que el desbloqueo se realiza únicamente vía correo electrónico. |
| **RF13** | **Errores de Conexión** | Detectar falta de internet o timeout (10 seg) y mostrar el mensaje: "No podemos conectarnos a internet, por favor revise su conexión". |
| **RF14** | **Menú de Navegación** | Incluir una barra inferior fija (Bottom Navigation Bar) con acceso a Inicio, Pases, Expediente y Citas. |
| **RF15** | **Buscador de Derechohabientes** | Filtro en tiempo real a partir de 3 caracteres, insensible a mayúsculas, minúsculas y acentos. |
| **RF16** | **Configuración** | Mostrar el correo del usuario logueado y enlaces externos al Aviso de Privacidad y Manual de Operaciones. |

---

## 2. Requisitos No Funcionales (RNF) - Usabilidad y Accesibilidad

Estos requisitos están diseñados para mitigar las barreras tecnológicas de los **Usuarios Manuales** y la fatiga visual del **Personal Docente/Administrativo (45-70 años)**.

| ID | Atributo | Especificación |
| :--- | :--- | :--- |
| **RNF-U-01** | **Legibilidad** | La interfaz debe soportar el escalado de fuentes del sistema operativo, manteniendo un tamaño base de **16px** para garantizar la lectura en el rango de edad de 45-70 años. |
| **RNF-U-02** | **Contraste** |El diseño debe cumplir con el nivel **AA (WCAG 2.1)** con un ratio de contraste mínimo de 4.5:1 para reducir la fatiga visual. |
| **RNF-U-03** | **Interactividad** | Los botones y elementos clicables deben tener un área mínima de **44x44 dp** para facilitar la pulsación a usuarios con menor experiencia digital. |
| **RNF-U-04** | **Carga Cognitiva** | El flujo de agendado debe emplear revelación progresiva, mostrando un máximo de 3 campos por pantalla para evitar saturar al usuario. |
| **RNF-U-05** | **Navegación Clara** | Los iconos del menú inferior (RF14) deben incluir etiquetas de texto obligatorias para asegurar que la interfaz no requiera habilidades organizativas avanzadas. |
| **RNF-U-06** | **Mensajes Humanos** | Los errores deben describirse en lenguaje natural y no técnico, explicando siempre el paso a seguir para solucionar el inconveniente. |
| **RNF-U-07** | **Feedback Visual** | Ante cualquier acción que dure más de 200ms, el sistema debe mostrar un indicador de carga para mitigar la ansiedad ante interfaces digitales. |