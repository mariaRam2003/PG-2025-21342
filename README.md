# ARTour Virtual (AR Tour App V2)

## Descripción

Aplicación de recorridos virtuales con Realidad Aumentada (AR), desarrollada en Unity y diseñada para la Universidad del Valle de Guatemala. Esta nueva versión integra mejoras en navegación con sensores UWB, accesibilidad y usabilidad.

Brinda una experiencia interactiva que combine recorridos físicos con información digital aumentada, integrando Realidad Aumentada, sensores UWB Beacon para posicionamiento, interfaz intuitiva y responsive en iOS (y multiplataforma en fases futuras), y funcionalidades de gamificación con minijuegos.

## Características Principales

- Navegación en interiores con beacons UWB de Estimote
- Pathfinding en tiempo real usando NavMesh de Unity
- Asistente de voz como guía virtual (Google TTS)
- Interfaz responsiva con UI Toolkit
- Minijuegos integrados para gamificación de la experiencia

## Tecnologías Utilizadas

- Unity 6.000.0.55f1
- SDK Estimote UWB Beacons
- UI Toolkit (UXML + USS)
- Google TTS
- NavMesh de Unity
- .NET Framework
- Xcode (para compilaciones móviles)

## Requisitos Previos

- Unity 6.000.0.55f1 o superior
- SDK Estimote UWB Beacons
- Xcode (para compilaciones iOS)
- .NET Framework compatible con Unity
- Unity Hub

## Instalación

1. Clonar el repositorio:
```bash
   git clone https://github.com/AR-Tour-UVG/AR-Tour-V2.git
   cd AR-Tour-V2
```

2. Abrir el proyecto en Unity Hub

3. Seleccionar la escena principal:
```
   Assets/Scenes/PantallaPrincipal.unity
```

4. Ejecutar el proyecto:
   - En Play Mode para pruebas en editor
   - Compilar para iOS desde Build Settings

## Estructura del Proyecto
```
ARTour/
├── Assets/
│   ├── UI/             # Pantallas .uxml y estilos .uss
│   ├── Scripts/        # Lógica en C#
│   ├── Minijuegos/     # Juegos heredados de versiones anteriores
│   ├── Scenes/         # Escenas de Unity
│   └── Resources/      # Imágenes, fuentes y materiales
│
├── Docs/               # Documentación extendida en Markdown
├── Packages/           # Dependencias de Unity
├── ProjectSettings/    # Configuración del proyecto
└── README.md           # Este archivo
```

## Arquitectura

- **UI Toolkit (UXML + USS)** para interfaz de usuario
- **CambiadorDePantallas.cs** gestiona navegación entre pantallas
- **Módulo UWB Beacons** (en desarrollo) para posicionamiento en interiores
- **Módulo Minijuegos** importado y adaptado de versiones anteriores

### Pantallas Principales

- **PantallaInicio**: Menú principal
- **PantallaEscaneo**: Conexión a sensores UWB Beacon (con bypass de prueba)
- **PantallaARTour**: Vista AR con información de ubicación, nivel, ruta e instrucciones
- **PantallaMinijuegos**: Acceso a juegos interactivos como Breakout, FlappyJack y Trivia

## Control de Versiones

Este proyecto utiliza Unity Version Control integrado con GitHub:

- El repositorio de GitHub y Unity Version Control están sincronizados automáticamente
- Los commits realizados en Unity Version Control se reflejan automáticamente en GitHub
- Esto permite un flujo de trabajo colaborativo eficiente entre desarrolladores

## Demo

El video demostrativo se encuentra en `/demo/demo.mp4`

## Documentación

La documentación completa (manual de usuario, manual técnico y guías de instalación) se encuentra disponible en `/Docs/`

## Futuro del Proyecto

- Migración completa a multiplataforma (Android + iOS)
- Integración real de sensores UWB Beacon
- Optimización de minijuegos
- Implementación de panel de administración para gestión de rutas

## Autores

- Diego Alberto Leiva
- Gustavo Andres Gonzalez Pineda
- Maria Marta Ramírez
- Eduardo Ramírez

## Licencia

MIT LICENSE
