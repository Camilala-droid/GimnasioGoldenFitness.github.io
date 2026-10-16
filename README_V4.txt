GOLDEN FITNESS V4 - MEJORA VISUAL Y FLUJO OPERATIVO
===================================================

Objetivo: mantener PHP MVC entendible para colegio, pero con una interfaz más profesional y flujos conectados.

MEJORAS PRINCIPALES
- Foto de cliente y entrenador (JPG/PNG/WEBP, máximo 3 MB).
- Ficha visual del cliente y perfil profesional del entrenador.
- Clases en tarjetas visuales con categoría, color, foto del entrenador, especialidad y horarios.
- CRUD de categorías de clase.
- CRUD de salas.
- Ticket imprimible de pago.
- Ticket imprimible de reserva.
- Credencial imprimible del cliente.
- Evaluación física imprimible.
- Rutina imprimible.
- Reportes con Imprimir/Guardar PDF desde navegador.
- Exportación CSV compatible con Excel: pagos, clientes, membresías, reservas y asistencias.
- Paleta, tarjetas, badges, formularios y jerarquía visual reforzados.

FLUJO PRINCIPAL
Cliente -> Membresía -> Pago -> Ticket -> Reserva -> Ticket -> Asistencia -> Evaluación -> Rutina -> Reportes.

FLUJO DE CLASES
Categoría -> Clase -> Entrenador -> Horario -> Sala -> Reserva -> Asistencia.

INSTALACIÓN NUEVA
1. Copiar la carpeta a C:\xampp\htdocs\golden_fitness
2. Importar database/golden_fitness.sql en phpMyAdmin.
3. Abrir http://localhost/golden_fitness/public/
4. Usuario: admin / Contraseña: admin123

ACTUALIZACIÓN DESDE V3
- Hacer respaldo de la BD.
- Ejecutar database/actualizacion_v3_a_v4.sql.
- Reemplazar los archivos del sistema por V4.

IMPRESIÓN Y PDF
Los comprobantes/reportes usan la impresión del navegador. Elegir "Guardar como PDF" para generar PDF sin librerías externas.

EXCEL
La exportación genera CSV UTF-8 separado por punto y coma, que Excel abre directamente.
