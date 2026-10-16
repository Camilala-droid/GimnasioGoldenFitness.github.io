GOLDEN FITNESS V3 - MVC PHP / MySQL
===================================

INSTALACION XAMPP
1. Copiar la carpeta golden_fitness_v3 dentro de C:\xampp\htdocs\
   Puede renombrarla como golden_fitness si desea.
2. Iniciar Apache y MySQL.
3. Abrir phpMyAdmin.
4. Importar database/golden_fitness.sql
5. Abrir:
   http://localhost/golden_fitness_v3/public/

USUARIO INICIAL
Usuario: admin
Contraseña: admin123

IMPORTANTE
La base V3 fue rediseñada y contiene 17 tablas. Para probar esta versión se recomienda importar el SQL desde cero.

MODULOS VISIBLES
- Dashboard
- Clientes y ficha del cliente
- Planes
- Membresías
- Pagos
- Entrenadores
- Clases
- Agenda / Horarios
- Reservas
- Asistencia
- Evaluaciones físicas
- Rutinas
- Reportes

FLUJO DE ESTUDIO
Vista -> Controlador -> Modelo -> Base de datos

Flujo de negocio:
Cliente -> Membresía -> Pago -> Reserva/Acceso -> Seguimiento -> Reportes
