[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/0Yg6oblj)

# Cegados por la IA

> "Ver el mundo a través de la voz."

**Cegados por la IA** es un sistema de inteligencia artificial diseñado para convertir, en tiempo real, la grabación de vídeo de unas gafas inteligentes en descripciones de audio para personas con discapacidad visual.

## 1. Descripción del proyecto

El proyecto busca resolver la dependencia tecnológica y mejorar la autonomía de las personas ciegas mediante un asistente visual avanzado. [cite_start]A diferencia de otras soluciones conectadas a la nube, nuestro sistema prioriza la **privacidad por diseño** y la **disponibilidad inmediata**[cite: 7, 157].

[cite_start]El sistema funciona mediante **procesamiento 100% local (Edge AI)**, analizando el entorno directamente en el hardware de las gafas sin enviar imágenes a servidores externos[cite: 20, 100]. [cite_start]Combina visión por computador, modelos de lenguaje (LLM) y síntesis de voz para describir obstáculos, leer textos y narrar el entorno social, garantizando que los datos personales sean efímeros y nunca se almacenen[cite: 18, 32, 37].

## 2. Control de versiones y nomenclatura de documentos

Para mantener un orden claro en la documentación, se seguirá la siguiente convención de nombres:

`NombreDelDocumento vx.y.ext`

- `NombreDelDocumento`: Descripción breve del contenido del documento.  
- `x`: Número del sprint en el que se crea o actualiza el documento.  
- `y`: Versión del documento dentro de ese sprint.  
- `ext`: Extensión del archivo (.pdf, .docx, .md, etc.).  

**Ejemplo:**

- `Especificacion v1.0.pdf` → Primer documento de especificación técnica del sprint 1.  
- `Propiedad Intelectual v2.1.docx` → Segunda versión del documento sobre PI en el sprint 2.  

## 3. Arquitectura y Privacidad

[cite_start]El sistema se basa en una arquitectura de **Edge AI** para garantizar que ningún dato biométrico o visual salga del dispositivo del usuario[cite: 100, 114].

### Flujo de Datos
1.  [cite_start]**Captura:** Módulo de cámara y sensores (giroscopio/GPS)[cite: 19, 21].
2.  [cite_start]**Filtrado:** Módulo de Contexto y Privacidad que detecta zonas sensibles (baños, vestuarios) para desactivar la cámara automáticamente[cite: 27, 8].
3.  **Procesamiento IA:**
    - [cite_start]Visión por Computador (CV) para estructurar datos (objetos, texto)[cite: 30, 32].
    - [cite_start]Modelo de Lenguaje (LLM) para generar la descripción[cite: 33].
4.  [cite_start]**Salida:** Síntesis de voz (TTS) a través de altavoces de conducción ósea[cite: 37, 39].

### Bucle de Privacidad
[cite_start]Garantizamos un ciclo de vida de los datos efímero[cite: 41]:
- [cite_start]**NO Almacenamiento:** Las imágenes se procesan y destruyen en milisegundos[cite: 42, 44].
- [cite_start]**NO Identificación:** Difuminado automático de rostros y matrículas; el sistema describe presencia humana sin identificar individuos[cite: 43, 97].
- [cite_start]**Eliminación Inmediata:** Al finalizar la sesión, se borran automáticamente todos los datos temporales y de configuración[cite: 91].

## 4. Licencias y Propiedad Intelectual

[cite_start]El proyecto utiliza un modelo híbrido para equilibrar la colaboración abierta con la seguridad del usuario[cite: 138, 139]:

- [cite_start]**Código Principal:** Licencia propietaria (protección contra vigilancia masiva y reventa)[cite: 133].
- [cite_start]**Módulo de Visión:** Licencia MIT (fomenta compatibilidad con OpenCV/PyTorch)[cite: 134].
- [cite_start]**Modelo Neuronal:** CC BY-NC (uso no comercial para evitar explotación sin ética)[cite: 135].
- [cite_start]**Datos:** CC BY-NC-SA (uso académico)[cite: 136].

## 5. Créditos y roles

Integrantes del equipo *Cegados por la IA*:

| Rol | Miembro | Responsabilidades |
| :--- | :--- | :--- |
| *Product Owner* | **Carmen** Fernández González | [cite_start]Visión del producto y gestión de requisitos[cite: 3]. |
| *Team Advocate* | **Diego** Alonso Arceiz | [cite_start]Defensa del equipo y bienestar del grupo[cite: 95]. |
| *Scrum Master* | **Ignacio** Gutiérrez Sánchez | [cite_start]Facilitador de la metodología ágil y eliminación de bloqueos[cite: 3]. |
| *Experto Git* | **Bryan** Xavier Quilumba | [cite_start]Gestión del repositorio, control de versiones y buenas prácticas[cite: 3]. |

