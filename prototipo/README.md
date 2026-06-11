# Prototipo Funcional — Sistema Aduana EP3

## Herramienta utilizada
**Figma** — Prototipado de alta fidelidad con navegación interactiva.

## Link del prototipo navegable
https://www.figma.com/make/1F5SUtF485joOMOzVwVMaz/Sistema-Aduana-EP3?fullscreen=1&t=YzKIVUhgkffcLKlC-1&code-node-id=0-9

## Pantallas implementadas
| # | Pantalla | Requisito cubierto |
|---|----------|--------------------|
| 1 | Login institucional | RNF — Seguridad / cuenta habilitada |
| 2 | Dashboard principal | RF — Panel central con módulos |
| 3 | Registro de Viajero | RF — Ingreso de datos del viajero |
| 4 | Módulo Menores | RF — Autorización notarial menores de edad |
| 5 | Módulo Vehículos | RF — Admisión temporal 180 días |
| 6 | Revisión SAG | RF — Declaración productos agrícolas/animales |
| 7 | Revisión PDI | RF — Validación migratoria |
| 8 | Vista Integrada | RF — Resumen SAG + PDI + Menores |
| 9 | Autorización Final | RF — Comprobante de cruce |
| 10 | Informes y Estadísticas | RF — Reportes con gráficos y exportar PDF |

## Requisitos no funcionales implementados
- **Seguridad:** Login con validación de cuenta habilitada
- **Usabilidad:** Interfaz intuitiva con colores institucionales Aduana Chile (#003366)
- **Eficiencia:** Flujo digitalizado, trámite completo en menos de 5 interacciones
- **Portabilidad:** Accesible desde cualquier navegador web

## Flujo de navegación
```
Login → Dashboard → Registro Viajero → Menores → Vehículos → SAG → PDI → Vista Integrada → Autorización Final
Dashboard → Informes y Estadísticas
```
