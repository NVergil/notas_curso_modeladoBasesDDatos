# Maratones
<!-- Recordar las entidades se nombran en plural y los atributos en singular -->
<!-- 
**(PK)** Primary Key
**(FK)** Foreign Key
**(ED)** Entity Data
**(EC)** Entity Catalog
 -->

## Listado de Entidades

### carreras **(ED)** 

- carrera_id **(PK)**
- nombre
- tipo_carrera **(FK)**
- fecha
- tiempo
- mejor_tiempo
- altitud
- lugar
- pais **(FK)**
- foto

### tipos_carreras **(EC)**

- tipo_carrera_id **(PK)**
- descripcion 
- distancia **(UQ)**

### paises **(EC)**

- pais_id **(PK)**
- nombre

## Relaciones

1. Una **carrera** _pertenece_ a un **tipo de carrera** (_1 a 1_).
2. Una **carrera** se _corre_ en un **país** (_1 a 1_).

### Modelo Entidad - Relación

![Modelo Entidad - Relación](./Designes_PNG%26drawio/CarrerasModeloEntidad-Relacion.drawio.png)

### Modelo Relacional de la BD

![Modelo Entidad - Relacion](./Designes_PNG%26drawio/ModeloRelacional-de-la-BD.png)

## Reglas de Negocio

### carreras

1. Crear el registro de una carrera
1. Leer el registro de una(s) carrera(s) dada una condicion en particular.
1. Leer todos los registros de la entidad carreras.
1. Actualizar los datos de una carrera dada una condicion en particular.
1. Eliminar los datos de una carrera dada una condicion en particular.

### tipos_carreras

1. Crear el registro de un tipo de carrera
1. Leer el registro de uno(s) tipo(s) de carrera(s) dada una condicion en particular.
1. Leer todos los registros de la entidad tipos carreras.
1. Actualizar los datos de un tipo de carrera dada una condicion en particular.
1. Eliminar los datos de un tipo carrera dada una condicion en particular.

### paises

1. Crear el registro de un pais
1. Leer el registro de uno(s) tipo(s) de carrera(s) dada una condicion en particular.
1. Leer todos los registros de la entidad tipos carreras.
1. Actualizar los datos de un tipo de carrera dada una condicion en particular.
1. Eliminar los datos de un tipo carrera dada una condicion en particular.