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

#### 1. Realice el diagrama de contexto con las generalidades de su sistema.
(Añadirlo al README.md)

Respuesta:

<img width="865" height="649" alt="image" src="https://github.com/user-attachments/assets/729af901-f3f8-4753-9fd3-859d7ec01469" />

#### 2. Identifique 2 patrones de diseño que puedan aplicarse al caso de estudio,
especificando por cada uno:

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







