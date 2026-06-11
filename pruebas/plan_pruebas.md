# Plan de Pruebas — Sistema Aduana EP3
## Norma: ISO/IEC 25000 + ISO9126

---

## 1. Objetivo
Verificar que el prototipo funcional del Sistema de Aduana cumple los requisitos funcionales y no funcionales definidos en el caso, aplicando el modelo de calidad ISO9126 como marco de evaluación y el estándar ISO25000 como guía de proceso.

## 2. Alcance
El plan cubre las siguientes funcionalidades del prototipo:
- Login institucional con validación de cuenta
- Registro de viajeros
- Documentación de menores de edad
- Trámite de vehículos (admisión temporal)
- Revisión SAG (productos agrícolas y animales)
- Revisión PDI (validación migratoria)
- Vista integrada y autorización de cruce
- Informes estadísticos con exportación PDF

## 3. Normas utilizadas
| Norma | Aplicación |
|-------|-----------|
| **ISO/IEC 25000 (SQuaRE)** | Marco general de evaluación de calidad del producto de software |
| **ISO/IEC 9126** | Modelo de características de calidad aplicado al prototipo |

## 4. Características de calidad evaluadas (ISO9126)
| Característica | Definición aplicada | Módulo evaluado |
|----------------|--------------------|-----------------| 
| **Funcionalidad** | El sistema ejecuta correctamente todas las operaciones del caso | Todos los módulos |
| **Eficiencia** | El flujo digitalizado reduce el tiempo de trámite | Flujo completo |
| **Fiabilidad** | Validaciones y estados reducen errores de tramitación | Menores, SAG, PDI |
| **Seguridad** | Solo usuarios con cuenta habilitada acceden al sistema | Login |
| **Usabilidad** | Interfaz clara e intuitiva con colores institucionales | Todas las pantallas |
| **Mantenibilidad** | Componentes reutilizables y versiones documentadas | Figma + Git |
| **Portabilidad** | Accesible desde cualquier navegador web | Prototipo web |

## 5. Estrategia de pruebas
- **Tipo:** Pruebas funcionales + pruebas de interfaz de usuario
- **Método:** Caja negra — se verifica el comportamiento observable del prototipo
- **Ambiente:** Prototipo navegable en Figma, visualizado desde navegador web (Chrome)
- **Evidencias:** Capturas de pantalla de cada caso de prueba ejecutado

## 6. Criterios de aceptación
- **Aprobado (Pass):** El resultado obtenido coincide exactamente con el resultado esperado
- **Fallido (Fail):** El resultado obtenido difiere del esperado o no es posible ejecutar el caso

## 7. Responsables
| Rol | Responsable |
|-----|-------------|
| Ejecución de pruebas | [Integrante 1] |
| Registro de evidencias | [Integrante 2] |
| Revisión y aprobación | [Integrante 3] |

## 8. Relación Requisito ↔ Caso de Prueba
| ID Caso | Requisito | Característica ISO9126 | Módulo |
|---------|-----------|----------------------|--------|
| CP-01 | RF01 — Login habilitado | Seguridad | Login |
| CP-02 | RF01 — Login no habilitado | Seguridad / Fiabilidad | Login |
| CP-03 | RF04 — Menor con autorización | Funcionalidad | Módulo Menores |
| CP-04 | RF05 — Vehículo sin patente | Fiabilidad | Módulo Vehículos |
| CP-05 | RF06 — Productos SAG restringidos | Funcionalidad | Módulo SAG |
| CP-06 | RF10 — Informe estadístico | Funcionalidad / Eficiencia | Informes |
| CP-07 | RNF — Colores institucionales | Usabilidad | Todas las pantallas |
