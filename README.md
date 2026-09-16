# Sonrisa Odontología (demo)

Sitio de una sola página para "Sonrisa", consultorio odontológico ficticio en Formosa Capital, Argentina. Pieza de demo/portfolio de [CEDETEC Digital](https://cedetec-digital.netlify.app/), pensada como caso representativo para prospección de profesionales independientes (dentistas, abogados, kinesiólogos, y consultorios en general).

No representa un negocio real: nombre, dirección, teléfono, profesionales y contenido son de ejemplo. Repo y sitio completamente independientes de otros proyectos de demo del portfolio (restaurante, barbería, tienda de ropa, gimnasio, rotisería): no comparten código, carpeta ni historial.

## Contenido

Sitio estático de un solo archivo (`index.html`, sin dependencias de build ni backend):

- Tratamientos con duración y precio de referencia.
- Sistema de turnos de 5 pasos (tratamiento → profesional → fecha y hora → datos del paciente, incluyendo obra social opcional → confirmación), con disponibilidad de horarios simulada de forma determinística.
- Al confirmar: mensaje de WhatsApp pre-cargado, descarga a calendario (`.ics`) y panel "Mis próximos turnos" con cancelación, todo persistido en `localStorage`.
- Equipo de profesionales y listado de obras sociales aceptadas.

Este mismo esqueleto (sistema de turnos, tratamientos, profesionales, obras sociales) es fácilmente adaptable a otros rubros de servicios profesionales: abogados (áreas de práctica en vez de tratamientos), kinesiólogos, psicólogos, veterinarias, etc.

## Deploy

Al ser HTML estático, se puede publicar directo en GitHub Pages, Netlify o Vercel apuntando a la raíz del repo.
