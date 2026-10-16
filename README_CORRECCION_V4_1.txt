GOLDEN FITNESS V4.1 - CORRECCIÓN DE COMPATIBILIDAD
===================================================

Esta revisión corrige los errores observados al usar los archivos V4 sobre una base de datos V3 existente:

1. Fatal error: Unknown column 'e.foto' in Clase.php.
2. Warning: Undefined array key 'descripcion' en Entrenadores.
3. Warning / salida dañada en Categorías por ausencia del campo color.

CAUSA
-----
Los archivos PHP eran V4, pero la base de datos instalada seguía con parte del esquema V3.
V4 agregó estos campos:
- clientes.direccion
- clientes.foto
- entrenadores.foto
- entrenadores.descripcion
- categorias_clase.color

SOLUCIÓN EN V4.1
----------------
El sistema ahora comprueba esos campos al entrar por public/index.php y, si faltan, los agrega automáticamente.
Esto permite actualizar copiando los archivos V4.1 sobre una instalación V3 sin tener que reinstalar toda la base.

Si el usuario MySQL no tiene permiso ALTER, el sistema mostrará una pantalla clara solicitando importar:
  database/actualizacion_v3_a_v4.sql

RECOMENDACIÓN
-------------
Para una instalación nueva, importe database/golden_fitness.sql.
Para una instalación ya usada con V3, simplemente copie V4.1 y abra el sistema; la compatibilidad se aplica automáticamente.
