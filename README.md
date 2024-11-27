# FERRE-JUNIOR
Manual de Usuario
Introducción
El sistema FERRE-JUNIOR es una plataforma para gestionar inventarios, proveedores e informes de forma sencilla y eficiente. Este manual te guiará sobre cómo utilizar las funciones principales del sistema.
Secciones del Sistema
1.	Inicio de Sesión
o	Ingresa el Usuario y la Clave para acceder al menú principal.
o	Credenciales predeterminadas:
	Usuario: admin
	Clave: 1234
2.	Menú Principal
o	Contiene enlaces para acceder a:
	Stock: Gestión de inventarios.
	Proveedores: Registro y consulta de proveedores.
	Informes: Generación de reportes.
3.	Stock
o	Visualiza los artículos en inventario.
o	Registra un nuevo artículo llenando los campos:
	ID, Nombre, Fecha de Registro, Proveedor, y Disponibilidad.
o	Haz clic en Registrar para agregarlo a la tabla.
4.	Proveedores
o	Consulta la lista de proveedores registrados.
o	Registra un nuevo proveedor llenando los campos:
	NIT, Nombre, Correo, y Especialidad.
o	Haz clic en Registrar para agregarlo a la tabla.
5.	Informes
o	Consulta los informes generados.
o	Registra un nuevo informe llenando los campos:
	Nombre del Informe, Fecha, y Descripción.
o	Haz clic en Registrar Informe para agregarlo a la tabla.
Notas Importantes
•	Asegúrate de completar todos los campos antes de registrar nuevos datos.
•	Los datos ingresados se agregarán directamente a la tabla visible en cada sección.

















Manual Técnico
Introducción
Este documento está dirigido a desarrolladores y técnicos que quieran comprender o extender la funcionalidad de la página web FERRE-JUNIOR.
Arquitectura del Proyecto
•	Tecnologías Usadas:
o	HTML: Estructura de la página web.
o	CSS: Estilos y diseño visual.
o	JavaScript: Manejo de la lógica del cliente.
•	Archivos Principales:
o	index.html: Página de inicio de sesión.
o	menu.html: Menú principal.
o	stock.html: Gestión de inventarios.
o	provedor.html: Gestión de proveedores.
o	informes.html: Gestión de informes.
Estructura del Código
1.	index.html
o	Valida las credenciales en el formulario.
o	Redirige a menu.html tras un inicio de sesión exitoso.
o	Usa JavaScript para manejar el evento submit.
2.	menu.html
o	Navegación hacia las secciones del sistema mediante la función goToPage.
3.	stock.html, provedor.html, e informes.html
o	Cada archivo contiene:
	Formulario para registrar datos nuevos.
	Tabla dinámica con datos iniciales y espacio para nuevos registros.
o	JavaScript gestiona:
	Validación de campos requeridos.
	Creación de filas dinámicas en las tablas.
Instrucciones de Configuración
Estructura de Carpetas:
/proyecto
├── index.html
├── menu.html
├── stock.html
├── provedor.html
├── informes.html
├── assets/
│   ├── fondo.jpg
│   ├── stock-icon.png
│   ├── proveedor-icon.png
│   ├── informes-icon.png
1.	Requisitos del Navegador:
o	Soporte para HTML5 y JavaScript (todos los navegadores modernos).
2.	Personalización de Datos:
o	Para modificar los datos iniciales de las tablas, edita las secciones <tbody> en cada archivo.
Detalles de Implementación
1.	Validaciones de Formularios:
o	Implementadas mediante JavaScript:
	Verifica que no haya campos vacíos antes de registrar datos.
 

1.	Adición Dinámica de Datos:
o	Nuevos registros se crean directamente en el DOM utilizando createElement y innerHTML.
2.	Estilos:
o	CSS personalizado para cada sección.
o	Tablas con colores alternos y resaltado al pasar el mouse.
Recomendaciones para Extensión
1.	Persistencia de Datos:
o	Implementar almacenamiento en el servidor usando tecnologías como PHP o Node.js.
o	Alternativamente, usar LocalStorage para almacenar datos en el navegador.
2.	Validaciones Avanzadas:
o	Agregar validaciones para evitar duplicados en campos como ID o NIT.
3.	Mejoras Visuales:
o	Usar frameworks como Bootstrap para una experiencia más responsiva.

