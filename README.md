# databases-workshop-1

## Ejercicio 1: Identificación de Entidades y Relaciones

**Descripción:**

- **Identificar** las entidades principales, sus atributos y las relaciones entre ellas en un caso de estudio de un sistema de gestión de biblioteca.

**Historia de Usuario: Sistema de Gestión de Biblioteca**

- En una biblioteca, los usuarios pueden tomar prestados libros. Cada libro tiene un título, un autor y una fecha de publicación. Los usuarios tienen un nombre, una dirección y un email. Cada vez que un usuario toma prestado un libro, se registra un préstamo, incluyendo la fecha de préstamo y la fecha de devolución.

**Objetivos:**

- **Recordar** los conceptos básicos de entidades y relaciones en bases de datos.
- **Comprender** la estructura de una base de datos a través de la identificación de entidades, atributos y relaciones.
- **Aplicar** los conceptos de claves primarias (PK) y claves foráneas (FK).

**Actividades:**

1. **Lectura y Discusión:**

   - Leer la historia de usuario e identificar las entidades principales (`Libro`, `Usuario`, `Préstamo`).
   - Listar los posibles atributos de cada entidad.

2. **Identificación de Entidades y Atributos:**

   - Identificar y listar las entidades (`Libro`, `Usuario`, `Préstamo`).
   - Para cada entidad, listar al menos cinco atributos relevantes (`Título`, `Autor`, `Fecha de Publicación` para `Libro`; `Nombre`, `Dirección`, `Email` para `Usuario`; `Fecha de Préstamo`, `Fecha de Devolución` para `Préstamo`).

3. **Determinación de Claves:**

   - Identificar las claves primarias (PK) para cada entidad.
   - Identificar las claves foráneas (FK) que establecen las relaciones entre entidades (`Libro` a `Préstamo`, `Usuario` a `Préstamo`).
   
## Ejercicio 2: Comprensión de la Cardinalidad

**Descripción:**

- Explicación detallada de los diferentes tipos de cardinalidad utilizando ejemplos prácticos y gráficos.
- Los estudiantes analizarán la cardinalidad de las relaciones en el caso de estudio.

**Tipos de Cardinalidad:**

- **Uno a Uno (1:1):**

  - **Definición:** Cada entidad en el conjunto A se relaciona con una sola entidad en el conjunto B y viceversa.
  - **Ejemplo Real:** En una ciudad, cada persona tiene un único pasaporte, y cada pasaporte pertenece a una sola persona.
  - **Gráfico:**

<img src="assets/onetoone.png" alt="Ejemplo Uno a Uno" width="500px" />

- **Uno a Muchos (1:N):**

  - **Definición:** Una entidad en el conjunto A se relaciona con muchas entidades en el conjunto B.
  - **Ejemplo Real:** Un autor puede escribir muchos libros, pero cada libro tiene un único autor.
  - **Gráfico:**

<img src="assets/onetomany.png" alt="Ejemplo Uno a Muchos" width="500px" />


- **Muchos a Muchos (M:N):**
  - **Definición:** Muchas entidades en el conjunto A se relacionan con muchas entidades en el conjunto B.
  - **Ejemplo Real:** Los estudiantes pueden inscribirse en muchos cursos, y cada curso puede tener muchos estudiantes.
  - **Gráfico:**

<img src="assets/manytomany.png" alt="Ejemplo Muchos a Muchos" width="500px" />

**Objetivos:**

- **Comprender** los diferentes tipos de cardinalidad en las relaciones de bases de datos.
- **Aplicar** la cardinalidad adecuada a las relaciones identificadas en el caso de estudio.
   - Crear ejemplos adicionales en grupos donde los estudiantes definan entidades y relaciones con diferentes cardinalidades.
   - Presentar los ejemplos creados y explicar las decisiones tomadas.

## Ejercicio 3: Creación de un Modelo Relacional

**Descripción:**

- Los estudiantes crearán un modelo relacional basado en el caso de estudio del sistema de gestión de biblioteca.
- Deberán representar las entidades, atributos y relaciones, incluyendo las cardinalidades apropiadas.

**Historia de Usuario:**

- En la biblioteca, cada libro puede ser prestado muchas veces, pero cada préstamo corresponde a un único libro. Un usuario puede tomar prestados varios libros, y cada préstamo corresponde a un único usuario.

**Objetivos:**

- **Aplicar** los conocimientos adquiridos para diseñar un modelo relacional.
- **Crear** un modelo relacional claro y preciso.

**Actividades:**

1. **Revisión de Requerimientos:**

   - Revisar los requerimientos del caso de estudio.

2. **Diseño del Modelo Relacional:**
   - Utilizando una herramienta de diseño (por ejemplo, draw.io), crear un modelo relacional que incluya:
     - Entidades (`Libro`, `Usuario`, `Préstamo`) representadas por rectángulos.
     - Atributos de cada entidad representados por nombres de atributos dentro de los rectángulos.
     - Claves primarias (PK) y claves foráneas (FK) representadas por líneas y flechas.
     - Relaciones entre entidades representadas por líneas con la cardinalidad apropiada.
     - Cardinalidades de las relaciones (`Usuario` a `Préstamo`: 1:N; `Libro` a `Préstamo`: 1:N).

## Ejercicio 4: Casos Adicionales para Practicar y Afianzar el Aprendizaje

**Descripción:**

- Se presentarán 5 casos adicionales para que los estudiantes practiquen el diseño de modelos relacionales.

**Objetivos:**

- **Evaluar** la habilidad de los estudiantes para aplicar los conceptos aprendidos en nuevos contextos.
- **Crear** modelos relacionales completos y precisos para diferentes sistemas de información.

**Historias de Usuario:**

1. **Sistema de Gestión de Ventas:**

   - En una tienda, cada producto tiene un nombre y un precio. Los clientes realizan pedidos, y cada pedido puede incluir varios productos. Un cliente puede hacer muchos pedidos, y cada pedido pertenece a un único cliente.

2. **Sistema de Gestión de Hospital:**

   - En un hospital, cada paciente puede tener citas con varios médicos. Los médicos pueden atender a muchos pacientes. Cada cita incluye la fecha de la cita y el diagnóstico.

3. **Sistema de Gestión de Universidad:**

   - En una universidad, los estudiantes se inscriben en cursos. Cada curso tiene un nombre y un código. Los estudiantes pueden estar inscritos en muchos cursos, y cada curso puede tener muchos estudiantes inscritos.

4. **Sistema de Gestión de Recursos Humanos:**

   - En una empresa, los empleados trabajan en proyectos. Cada proyecto tiene un nombre y una fecha de inicio. Un empleado puede trabajar en varios proyectos, y cada proyecto puede tener varios empleados asignados.

5. **Sistema de Gestión de Inventario:**

   - En un almacén, los productos son suministrados por proveedores. Cada producto tiene un nombre y una cantidad en stock. Un proveedor puede suministrar muchos productos, y cada producto puede ser suministrado por varios proveedores.
