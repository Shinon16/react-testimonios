# Aplicación de Testimonios con React

## 1. Descripción del proyecto

Proyecto desarrollado para la asignatura de Ingeniería de Software, Unidad 3, periodo agosto–diciembre de 2026.

La aplicación permite consultar testimonios ficticios de clientes mediante una interfaz desarrollada con React y Vite.

El propósito de la práctica es comprender el desarrollo basado en componentes, el uso de props, eventos, estado y renderizado, así como aplicar técnicas de desarrollo colaborativo mediante Scrum y Pair Programming.

**Historia de usuario:**

Como visitante de un sitio web, quiero consultar testimonios de clientes mediante controles de navegación para conocer sus experiencias con el servicio.

## 2. Integrantes

- [Christian Raul Paramo Bautista]
- Pablo [apellido]

**Metodología:** Scrum y técnicas de Extreme Programming (XP), especialmente Pair Programming.

Los integrantes alternarán los roles de Driver (conductor) y Navigator (observador), registrando los cambios y revisiones realizados durante la práctica.

## 3. Tecnologías utilizadas

| Herramienta | Versión o propósito |
|---|---|
| React | Biblioteca para construir interfaces mediante componentes |
| Vite | 8.3.6 |
| Node.js | 24.20.0 |
| npm | 11.19.0 |
| JavaScript | Lógica de componentes e interacciones |
| CSS | Diseño y adaptación responsive |
| Visual Studio Code | Editor de código |
| Git y GitHub | Control de versiones y colaboración |

**Entorno:** Windows con terminal PowerShell.

## 4. Instalación y ejecución

1. Clonar el repositorio de GitHub.
2. Abrir una terminal dentro de la carpeta del proyecto.
3. Ejecutar `npm install` para instalar las dependencias.
4. Ejecutar `npm run dev` para iniciar el servidor de desarrollo.
5. Abrir la dirección local proporcionada por Vite, normalmente `http://localhost:5173/`.

Para generar la versión de producción, ejecutar `npm run build`.

## 5. Estructura principal

- `index.html`: punto de entrada HTML.
- `src/main.jsx`: monta la aplicación React.
- `src/App.jsx`: coordina el estado, la navegación y los componentes.
- `src/data.js`: contiene los testimonios ficticios.
- `src/components/Testimonial.jsx`: muestra la información de cada testimonio.
- `src/components/Controls.jsx`: contiene los botones de navegación.
- `src/styles.css`: define el diseño responsive y los estilos de accesibilidad.

## 6. Funcionalidades desarrolladas

**Etapa básica:**

- Presentación de fotografía, nombre, cargo y comentario.
- Navegación mediante los botones Anterior y Siguiente.
- Selección de testimonios mediante el botón Aleatorio.
- Navegación circular entre el primer y el último registro.
- Contador de la posición actual.
- Manejo de uno o cero testimonios.
- Incorporación de cinco testimonios ficticios adicionales, para un total de ocho.
- Diseño adaptable a dispositivos móviles, tabletas y computadoras.
- Estilos de foco visible para los controles.

**Etapa de ampliación — Pendiente:**

- Reproducción automática cada cinco segundos.
- Botones Pausar y Reanudar.
- Detención del avance automático al navegar manualmente.
- Limpieza del temporizador mediante `useEffect`.

## 7. Decisiones de diseño

Se separaron los datos de la presentación para facilitar el mantenimiento.

El componente `App` conserva el índice mediante `useState`, mientras que `Testimonial` recibe el registro seleccionado mediante props.

El componente `Controls` recibe callbacks para comunicar las acciones del usuario.

Se implementó una validación para evitar acceder a registros inexistentes cuando el arreglo está vacío.

La interfaz utiliza Flexbox, unidades flexibles y una media query para adaptar los controles y tarjetas a diferentes tamaños de pantalla.

## 8. Registro de pruebas

| ID | Prueba | Resultado registrado |
|---|---|---|
| P01 | Mostrar el primer testimonio | Aprobado |
| P02 | Navegación Siguiente | Aprobado |
| P03 | Límite superior | Aprobado |
| P04 | Límite inferior | Aprobado |
| P05 | Selección aleatoria | Aprobado |
| P06 | Funcionamiento con un registro | Visualización comprobada; confirmar acciones de botones |
| P07 | Funcionamiento sin registros | Visualización aprobada |
| P08 | Ampliación a ocho testimonios | Ocho registros integrados; completar verificación de límites |
| P09 | Diseño responsive y accesibilidad | Tres tamaños y foco visible comprobados; confirmar activación por teclado |
| P10 | Compilación de producción | Aprobado; pendiente revisión de consola del navegador |

**Resultado de compilación:** 19 módulos transformados; compilación completada en 346 ms, sin errores de compilación.

## 9. Organización del trabajo

Tablero de trabajo con las columnas:

- Pendiente
- En proceso
- En revisión
- Terminado

**Avance inicial:** preparación del entorno, creación de componentes, carga de datos, navegación, estilos y primeras pruebas.

**Siguiente actividad:** reproducción automática con `useEffect`, a desarrollar en pareja, iniciando Pablo como Driver y su compañero como Navigator.

Se registrarán los cambios de roles, dificultades encontradas, revisiones y mejoras.

## 10. Evidencias y revisión

Evidencias obtenidas durante el desarrollo:

- Funcionamiento de la primera tarjeta.
- Navegación entre testimonios.
- Pruebas con uno y cero registros.
- Incorporación de los ocho testimonios.
- Capturas responsive en 320, 768 y 1280 píxeles.
- Evidencia de foco visible.
- Compilación de producción exitosa.

**Pendiente:** organizar las capturas en el repositorio, completar pruebas faltantes, registrar al menos una corrección o revisión, y solicitar revisión de otra pareja.

## 11. Estado del proyecto

**Etapa básica:** implementada, con verificaciones y revisión por completar.

**Reproducción automática:** pendiente de desarrollo y pruebas A01–A07.

**Publicación web:** opcional para esta práctica.

## 12. Reflexión y conclusiones

Pendiente de completar individualmente por cada integrante al terminar el desarrollo y la revisión del proyecto.
