# Análisis de ventas de julio — Farmacias LV

### Contexto

Farmacias LV contrató a un científico de datos porque notó que sus ventas en **julio** fueron más bajas de lo esperado. Para entender qué sucedió, se centralizó la información de diferentes reportes de ventas — los archivos de Excel usados en el análisis no están incluidos en este repositorio por contener información sensible. Los datos se limpiaron y se unificaron en una base de datos SQLite (`farmacias.db`) y en un cuaderno de Jupyter (el archivo `Untitled0.ipynb`).

### Historia

Imagina que eres el científico de datos de Farmacias LV. Te entregan cuatro reportes distintos y te piden una fotografía completa de lo que pasó en julio. Comienzas limpiando nombres de vendedores, homogeneizando formatos de fechas y sumando ventas de sucursales distintas. Luego creas una base de datos para poder hacer consultas rápidas.

En tu análisis descubres que:

- Los horarios **matutino (8:00–15:00)** y **vespertino (15:00–22:00)** tienen comportamientos distintos. La mayor caída de ventas se concentra en el turno vespertino en todas las sucursales.
- Hay días con ventas **inferiores a 3 000 MXN**. Estos días se agrupan alrededor de dos fines de semana consecutivos de julio. Las sucursales “Sucursal 1” y “Sucursal 2” son las más afectadas.
- Algunos vendedores tienen tickets promedio muy bajos, lo que indica que en esos horarios atendieron menos clientes o vendieron productos de bajo valor.

Esto es como cuando preparas un desayuno con poca energía: si no hay suficiente gente en la cocina (sucursales con menos personal) o si los ingredientes son los mismos de siempre (ofertas monótonas), el resultado es un plato que no sorprende ni satisface. En julio, Farmacias LV dejó de sorprender a sus clientes y se relajó en la atención durante las tardes.

### Conclusiones y acciones recomendadas

1. **Horario vespertino bajo rendimiento**. El análisis mostró que la caída de ventas se concentró de 15:00 a 22:00. Podría deberse a menor personal disponible o a que los empleados están cansados después del turno matutino.

   **Acción**: implementar un sistema de rotación de personal para que los empleados que atienden por la tarde estén descansados, y ofrecer incentivos para aumentar el entusiasmo en ese horario (p. ej. comisiones mayores por ventas vespertinas).

2. **Fin de semana crítico**. Dos fines de semana de julio tuvieron ventas menores a 3 000 MXN. Puede estar relacionado con falta de stock o con campañas de la competencia.

   **Acción**: revisar niveles de inventario antes de fines de semana, lanzar campañas de promociones específicas para esos días (“fin de semana de salud”), y realizar alianzas con proveedores para asegurar la disponibilidad de productos clave.

3. **Vendedores con bajo ticket promedio**. Algunos vendedores registraron tickets promedio menores al resto. Esto puede ser falta de capacitación o desconocimiento de los productos.

   **Acción**: capacitar a vendedores en técnicas de venta cruzada (ofrecer productos complementarios) y en actualización de productos nuevos. Implementar un programa de mentoría donde los mejores vendedores acompañen a los de menor desempeño.

4. **Sucursales inconsistentes**. Las sucursales “Sucursal 1” y “Sucursal 2” muestran mayor variabilidad en ventas. Tal vez atienden públicos diferentes o se encuentran en zonas con alta competencia.

   **Acción**: evaluar el entorno de cada sucursal y diseñar estrategias locales, como convenios con consultorios cercanos, venta de productos especializados y campañas de marketing digital geolocalizadas.

### Archivos incluidos

- `Untitled0.ipynb`: cuaderno de Jupyter con el código usado para limpiar los datos, crear la base SQLite y realizar consultas.
- `README.md`: este documento, que resume el análisis y propone acciones a seguir.

> **Nota:** Los archivos de datos originales no se incluyen por confidencialidad, pero el cuaderno explica el proceso de análisis y puede adaptarse a nuevas versiones de los datos.
