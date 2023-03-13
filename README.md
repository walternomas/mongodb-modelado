# Modelado de datos en MongoDB

## Metodología para el modelado de datos

### Restricciones

- Los documentos en MongoDB tienen un máximo de 16 MB de tamaño.

### Metodología

1. Requerimientos.
2. Identificar ER.
3. Aplicar patrones.

### Cada una de estas fases se rodea de ciertos aspectos.

- **_Escenario:_** Como serán los escenarios del modelo de negocio (Ej.: Como un usuario usará la app, dónde podrá editar sus mensajes o como comprará un producto).
- **_Expertos:_** Necesitamos expertos relacionados a nuestro tipo de negocio (Ej.: Si planeamos ofrecer un software orientado a la contabilidad necesitamos a un experto que nos explique los conceptos que debemos manejar para su desarrollo).
- **_Sistema actual:_** Tener en cuenta como funciona su sistema actual y analizar como llevan a cabo sus tareas (Ej.: Las empresas llevan una gestión de sus ventas en un excel).
- **_DB Admin:_** El experto en modelado que une todas estas características y llega a un _resultado_.

### Este resultado serían 3 cosas:

- **_Workload:_** Donde indentificamos la carga de trabajo, las operaciones importantes, el tamaño de los datos, las consultas y posibles suposiciones.
- **_Relaciones:_** Lo obtenemos a partir de los sistemas actuales y el experto en modelado de datos. Identifcamos las entidades, atributos, restricciones y relaciones.
- **_Patrones:_** Cuando tenemos el diagrama de entidad-relación identificamos los patrones en el modelo de negocio que nos permiten realizar optimizaciones de la carga de trabajo u obtener un mejor desempeño de la misma.

### Todo esto nos lleva a un Diseño.

#### Workload

- Tamaño de los datos.
- Consultas e índices.
- Operaciones importantes.
- Suposiciones.

#### Relaciones

- Identificar entidades.
- Identificar atributos.
- Identificar restricciones.
- Identificar relaciones.
- Embeber vs referenciar.

#### Patrones

- Identificar y aplicar.
