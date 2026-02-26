# DOSW_ParcialT1_JuanLaverde
### PARTE 2.2 – Caso de estudio: SILABINFO (65%)
#### Contexto general 
La decanatura de Ingeniería de Sistemas desea mejorar la experiencia de los
colaboradores del laboratorio para la gestión de laboratorios y salones de clase a
través de Silabinfo (herramienta que ya existe).
Actualmente, Silabinfo permite gestionar laboratorios y salones de clase, pero
desea extender su funcionalidad para administrar oficinas, salas de estudio y
equipos (computadores específicos, proyectores, apuntadores, etc.). Igualmente,
desea que las reservas puedan ser gestionadas directamente por parte de
profesores, estudiantes y monitores, sin requerir el apoyo directo de los
colaboradores del laboratorio.
Los tipos de recursos que se desean gestionar por medio de Silabinfo son:

● Laboratorios (Ej.: Ingeniería de Software, Redes, Infraestructura, etc).

● Salones de clase (Ej.: C-204)

● Oficinas (cubículos de la decanatura de sistemas).

● Salas de estudio (Ej.: Sala del B0).

● Equipos (Ej.: Computadores para sustentaciones de materias específicas).

#### 1. Realice el diagrama de contexto con las generalidades de su sistema
(Añadirlo al README.md)

Respuesta:

<img width="865" height="649" alt="image" src="https://github.com/user-attachments/assets/729af901-f3f8-4753-9fd3-859d7ec01469" />

#### 2. Identifique 2 patrones de diseño que puedan aplicarse al caso de estudio,especificando por cada uno:

a. Nombre del Patrón

b. Tipo de patrón (creacional, estructural o de comportamiento).

c. Justificación de la decisión.

Respuesta:
2.1 a) El primer patron que usare sera Factory Method contructor visual 

2.1 b) Este tipo de patron es de la categoria creacional 

2.1 c) Usare este patron de la categoria creacional ya que este es un patron que nos permite crear una interfaz para crear objetos en las superclases, esto nos permite actualizar el SILABINFO con sus categorias a la par para que visualmente se vean los cambios, esto permitiendonos mantener lo solicitado que era mantener el diseño alusivo al programa de ingeniera de sistemas a su vez que mantiene una tipologia apropiada

2.2) a) El segundo patron que usare para esto sera el de Builder 

2.2) b) Este tipo de patron es de la categoria estructural 

2.2) c) Usare este tipo de patron Builder ya que este nos permite crear/construir objetos de manera secuencial por lo que para la creacion y procesamiento de las listas en la base de datos ya que debido a la estructura de estas ejem: 2083853,LauraHerrera,laura.herrera@escuelaing.edu.c  para listas de personas o tambien para las de materias <img width="665" height="350" alt="image" src="https://github.com/user-attachments/assets/baf0e092-fd7e-4903-ab54-a5abbad9e081" />
Por lo que el uso de este patron nos permite agregar diferentes asignaturas de diferentes tipos y de diferentes plan de estudio a su vez que de su nivel por lo que el patron con una misma estructura nos permite crear varios objetos en sus categorias y asi poder ampliar y gestionar de una manera mas eficiente 

#### Identifique 5 requerimientos del sistema y clasifíquelos en funcionales (3) y no funcionales (2). Garantiza que al menos un requerimiento funcionalseleccionado utilice un patrón identificado. (Añadirlo al README.md) 

Respuesta: 

Requerimientos del sistema:

#### Requerimientos funcionales:

Gestión de reservas para diferentes tipos de recursos laboratorios, salones, oficinas, salas de estudio y equipo, Utiliza el patrón Factory Method para crear objetos de reserva según el tipo de recurso, permitiendo extender la funcionalidad de Silabinfo de manera flexible y escalable.

Validación de usuarios y reglas específicas para cada tipo de recurso:
El sistema debe validar si el usuario cumple con los requisitos profesor, monitor o estudiante y las reglas de tiempo, capacidad y disponibilidad antes de confirmar la reserva.

Integración con sistemas externos Enlace y Recursos Humanos:
Silabinfo debe obtener información de materias, profesores y estudiantes desde sistemas externos, validando que los datos cumplan con los formatos requeridos.

#### Requerimientos no funcionales:

Interfaz de usuario responsiva y con diseño alusivo al programa de Ingeniería de Sistemas:
La aplicación debe mantener colores y tipografía legibles, garantizando una experiencia de usuario agradable.

Alto rendimiento en la validación y procesamiento de reservas:
El sistema debe ser capaz de procesar las solicitudes de reserva en menos de 2 segundos, incluso con múltiples usuarios concurrentes.


####  Del listado anterior, seleccione los 2 requerimientos funcionales másimportantes del sistema y desarrolle un diagrama de casos de uso con surespectiva historia de usuario. Garantiza que al menos un requerimientofuncional seleccionado utilice un patrón identificado. (Añadirlo al README.md)

Respuesta:

<img width="998" height="372" alt="image" src="https://github.com/user-attachments/assets/07e67531-b94d-406d-931a-5cb6112ac6c9" />

<img width="903" height="163" alt="image" src="https://github.com/user-attachments/assets/cf4a2ffb-cdb6-4e30-8714-ec1159385fba" />

#### 
#### Requerimientos funcionales más importantes

Del listado anterior, se seleccionaron los siguientes dos requerimientos funcionales más importantes y se desarrollaron sus respectivos diagramas de casos de uso y sus historias de usuario.

---

### Requerimiento Funcional 1: Gestión de reservas de recursos

| Campo               | Descripción                                                                                     |
|---------------------|-------------------------------------------------------------------------------------------------|
| **ID**             | RF-01                                                                                          |
| **Nombre**         | Gestión de reservas de recursos                                                                |
| **Descripción**    | El sistema debe permitir a los usuarios realizar reservas de recursos como laboratorios, salones de clase, oficinas, salas de estudio y equipos, siguiendo las reglas específicas de cada tipo de recurso. |
| **Precondiciones** | Bankify debe tener previamente configurados los recursos disponibles y sus reglas de reserva.   |
| **Actor**          | Usuario (profesor, monitor o estudiante)                                                       |
| **Flujo principal**| 1. El usuario selecciona el tipo de recurso a reservar.<br>2. El sistema muestra los recursos disponibles según las reglas configuradas.<br>3. El usuario ingresa los datos de la reserva.<br>4. El sistema valida las reglas y confirma o deniega la reserva. |
| **Diagrama de caso de uso** | ![Diagrama RF-01](https://github.com/user-attachments/assets/07e67531-b94d-406d-931a-5cb6112ac6c9) |
| **Poscondiciones** | Se espera como resultado una reserva confirmada o una notificación de denegación con las razones correspondientes. |

---

### Requerimiento Funcional 2: Validación de usuarios y reglas de reserva

| Campo               | Descripción                                                                                     |
|---------------------|-------------------------------------------------------------------------------------------------|
| **ID**             | RF-02                                                                                          |
| **Nombre**         | Validación de usuarios y reglas de reserva                                                     |
| **Descripción**    | El sistema debe validar que los usuarios cumplan con los requisitos necesarios (profesor, monitor o estudiante) y que las reservas respeten las reglas de tiempo, capacidad y disponibilidad para cada tipo de recurso. |
| **Precondiciones** | Bankify debe tener previamente configurados los roles de usuario y las reglas específicas de cada recurso. |
| **Actor**          | Usuario (profesor, monitor o estudiante)                                                       |
| **Flujo principal**| 1. El usuario intenta realizar una reserva.<br>2. El sistema verifica el rol del usuario.<br>3. El sistema valida las reglas específicas del recurso solicitado.<br>4. El sistema confirma o deniega la reserva. |
| **Diagrama de caso de uso** | ![Diagrama RF-02](https://github.com/user-attachments/assets/cf4a2ffb-cdb6-4e30-8714-ec1159385fba) |
| **Poscondiciones** | Se espera como resultado una reserva válida o una notificación de denegación con las razones correspondientes. |

#### . Seleccione un requerimiento asociado al patrón y realice la descomposiciónde tareas asociadas: Épica - Historia de Usuario - Al menos 3 tareas. (Añadirlo al README.md)

Gestión de reservas de recursos
Como usuario, quiero realizar reservas de recursos laboratorios, salones, oficinas, salas de estudio y equipos para poder utilizarlos según mis necesidades, cumpliendo con las reglas específicas de cada tipo de recurso.

Historia de Usuario
Realizar una reserva de recurso Como usuario profesor, monitor o estudiante, quiero seleccionar un recurso y realizar una reserva, para asegurar su disponibilidad en el horario deseado 

El sistema debe permitir seleccionar el tipo de recurso laboratorio, salón, oficina, sala de estudio o equipo.
El sistema debe validar las reglas específicas del recurso seleccionado.
El sistema debe confirmar o denegar la reserva según las validaciones realizadas.

Tarea 1: Implementar el patrón Factory Method para la creación de objetos de reserva según el tipo de recurso.

Crear una clase base Reserva y subclases específicas para cada tipo de recurso 
Diseñar una fábrica que genere instancias de las subclases según el tipo de recurso seleccionado.

Tarea 2: Desarrollar la funcionalidad de validación de reglas específicas para cada tipo de recurso.

Implementar métodos de validación en las subclases de Reserva para verificar tiempo, capacidad y disponibilidad.
Integrar las validaciones con los datos obtenidos de sistemas externos 

Tarea 3: Crear la interfaz de usuario para la selección de recursos y la gestión de reservas.

Diseñar un formulario que permita al usuario ingresar los datos de la reserva 
Mostrar mensajes de confirmación o denegación según el resultado de las validaciones.
Esta descomposición asegura que el patrón Factory Method sea utilizado para gestionar la creación de reservas, mientras se desarrollan las validaciones y la interfaz de usuario necesarias para cumplir con la historia de usuario.





