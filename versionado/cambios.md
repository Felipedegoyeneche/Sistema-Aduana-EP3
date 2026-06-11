# Registro de Control de Cambios — Sistema Aduana EP3

## Historial de versiones del prototipo

| Versión | Fecha | Responsable | Descripción del cambio | Motivo / Requisito | Impacto |
|---------|-------|-------------|------------------------|--------------------|---------|
| V1.0 | 10-06-2026 | [Integrante 1] | Creación de login y dashboard principal | RF01 — Seguridad y acceso | Alto |
| V1.1 | 10-06-2026 | [Integrante 2] | Módulo de menores de edad con validación notarial | RF04 — Documentación menores | Alto |
| V1.2 | 10-06-2026 | [Integrante 3] | Módulo de vehículos (Sí/No + formulario admisión temporal 180 días) | RF05 — Vehículos | Medio |
| V1.3 | 10-06-2026 | Grupo | Registro de viajero + flujos SAG y PDI integrados | RF03, RF06, RF07 | Alto |
| V1.4 | 10-06-2026 | Grupo | Vista integrada SAG+PDI+Menores + Autorización Final con comprobante | RF08, RF09 | Alto |
| V1.5 | 10-06-2026 | Grupo | Módulo Informes y Estadísticas con gráficos y exportar PDF | RF10 — Reportes | Medio |

## Detalle de cambios por versión

### V1.0 — Login + Dashboard
- Pantalla de login con campos usuario/contraseña y validación de cuenta habilitada
- Dashboard con 5 módulos: Menores, Vehículos, SAG, PDI, Informes
- Colores institucionales Aduana Chile (#003366) aplicados
- **Justificación:** Base del sistema, cubre el requisito no funcional de seguridad más crítico

### V1.1 — Módulo Menores
- Formulario con nombre del menor, tipo de documento, autorización notarial (Sí/No)
- Badge de estado: Pendiente / Aprobado / Rechazado
- **Justificación:** Requisito explícito del caso — automatización de documentación de menores de edad

### V1.2 — Módulo Vehículos
- Bifurcación Sí/No para viajeros con o sin vehículo
- Formulario: patente, país de origen, propietario, tipo de documento (Salida temporal 180 días)
- Nota informativa sobre el plazo del documento
- **Justificación:** Cubre el Acuerdo Chileno-Argentino de admisión temporal

### V1.3 — Registro de Viajero + SAG + PDI
- Formulario de viajero con número de trámite auto-generado (ADU-...)
- SAG con checkboxes de productos agrícolas y animales
- PDI con validación migratoria y resultado final dropdown
- **Justificación:** Integra los tres servicios fiscalizadores del caso

### V1.4 — Vista Integrada + Autorización Final
- Resumen completo del trámite con estados de SAG, PDI y Menores
- Comprobante oficial con todos los datos del viajero
- Botones: Imprimir/Exportar PDF, Nuevo Trámite, Volver al Dashboard
- **Justificación:** Cierra el flujo completo del trámite aduanero

### V1.5 — Informes y Estadísticas
- Filtros por fecha y paso fronterizo
- Cards: Total Trámites, Aprobados, Rechazados, Pendientes
- Gráfico de barras (trámites por día) y gráfico circular (distribución por estado)
- Tabla detalle con número de trámite, viajero, fecha, paso fronterizo y estado
- Botón Exportar PDF
- **Justificación:** Cubre el requisito de generación de informes estadísticos automatizados
