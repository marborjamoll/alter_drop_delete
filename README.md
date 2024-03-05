# alter_drop_delete

# Modificando y Gestionando Tablas y Datos

## Objetivos de la Clase

- Entender el uso de los comandos `ALTER TABLE`, `ALTER COLUMN`, `DROP` y `DELETE` en SQL.
- Aprender a modificar estructuras de tablas existentes y gestionar datos dentro de las bases de datos.
- Practicar la creación y modificación de tablas y la gestión de datos a través de ejercicios.

## 1. Introducción a `ALTER TABLE` y `ALTER COLUMN`

### `ALTER TABLE`

El comando `ALTER TABLE` se utiliza para modificar la estructura de una tabla existente en la base de datos. Esto incluye añadir, modificar o eliminar columnas, así como modificar el tipo de datos de una columna existente.

#### Ejemplos:

- **Añadir una columna**: Para añadir una nueva columna a una tabla, se utiliza la siguiente sintaxis:

  ```sql
  ALTER TABLE nombre_tabla
  ADD nombre_columna tipo_datos;


- **Modificar una columna**: Para cambiar el tipo de datos de una columna existente, se utiliza:

   ```sql
  ALTER TABLE nombre_tabla
  MODIFY COLUMN nombre_columna nuevo_tipo_datos;

  Nota: En algunos sistemas de gestión de bases de datos (SGBD), ALTER COLUMN se utiliza específicamente para cambiar el tipo de datos o las restricciones de una columna existente. La sintaxis puede variar según el SGBD.

  ```sql
  ALTER TABLE nombre_tabla
  ALTER COLUMN nombre_columna SET DATA TYPE nuevo_tipo_datos;
  ```
   
- **Eliminar una columna**: Para eliminar una columna de una tabla, se utiliza:

  ```sql
  ALTER TABLE nombre_tabla
  DROP COLUMN nombre_columna;

## 2. Eliminando Datos y Estructuras: `DROP` y `DELETE`

### `DROP`

El comando `DROP` se utiliza para eliminar objetos de la base de datos, como tablas, vistas o índices.

#### Ejemplos:

- **Eliminar una tabla**: Para eliminar una tabla y todos sus datos permanentemente:

  ```sql
  DROP TABLE nombre_tabla;

- **Eliminar una base de datos**: Para eliminar una base de datos y todos sus datos permanentemente:

  ```sql
  DROP DATABASE nombre_tabla;

### `DELETE`

El comando `DELETE` se utiliza para eliminar registros específicos de una tabla, sin eliminar la tabla misma.

[Canción: No te olvides de poner el WHERE en el DELETE FROM](https://www.youtube.com/watch?v=i_cVJgIz_Cs)

#### Ejemplos:

- **Eliminar registros específicos**: Para eliminar registros que cumplan cierta condición:

  ```sql
  DELETE FROM nombre_tabla
  WHERE condicion;
  ```

- **Eliminar todos los registros**: Para eliminar todos los registros de una tabla sin eliminar la tabla:

  ```sql
  DELETE FROM nombre_tabla;

## 3. Ejercicios Propuestos

1. **Crear y Modificar una Tabla**: Dada una tabla `empleados` con columnas `id`, `nombre`, y `departamento`, añade una columna `email` y luego cambia el tipo de datos de `departamento` a `VARCHAR(100)`.
2. **Eliminar Columna**: Elimina la columna `email` de la tabla `empleados`.
3. **Eliminar Registros**: Elimina todos los registros de la tabla `empleados` que pertenezcan al departamento 'Recursos Humanos'.
4. **Eliminar una Tabla**: Elimina la tabla `empleados` de tu base de datos.
  
