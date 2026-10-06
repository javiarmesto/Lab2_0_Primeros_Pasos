# Mini Ejemplos para Usar Instrucciones Personalizadas

## Entrada por rol

- [Alumnado](EjercicioAlumnos.md): actividad y resultado que debes producir.
- [Instructor](InstruccionesInstructor.md): preparación y conducción del ejercicio.
- [Prompts de ejemplo](PromptsEjemplosAL.md): punto de partida para tu proyecto.

Es material docente y contexto de Copilot, no una extensión lista para publicar. Necesitas VS Code, AL Language, GitHub Copilot y un sandbox para compilar el código que generes. Crea un proyecto aparte con **AL: Go!**, configura tus versiones/IDs y `launch.json`, descarga símbolos y aplica las instrucciones del repo. El resultado esperado son objetos AL revisados y una prueba de sus validaciones en tu sandbox.

No hay manifiesto que fije versión BC; registra la de tu ejercicio. Inspección estática del 6 de octubre de 2026, sin compilar ni publicar.


## Descripción
Este repositorio contiene mini ejemplos diseñados para demostrar cómo utilizar instrucciones personalizadas en proyectos AL. Los ejemplos incluyen configuraciones iniciales y primeros prompts para facilitar el aprendizaje y la implementación.

## Contenido
- **Configuración Inicial**: Archivos y configuraciones básicas para comenzar.
- **Primeros Prompts**: Ejemplos de cómo interactuar con el sistema utilizando prompts personalizados.
- **Instrucciones Personalizadas**: Reglas de estilo y convenciones específicas para proyectos AL.

## Paso a Paso para Laboratorio
1. **Preparación del Entorno**:
   - Instala Visual Studio Code.
   - Configura la extensión AL Language.
   - Conéctate a un entorno de Business Central.

2. **Revisión de Archivos**:
   - Abre los archivos de ejemplo en el repositorio.
   - Familiarízate con las instrucciones personalizadas en [`.github/instructions/DemoCompanial.instructions.md`](.github/instructions/DemoCompanial.instructions.md).

3. **Ejecutar Prompts**:
   - Utiliza los prompts iniciales para explorar las funcionalidades.
   - Modifica los ejemplos según tus necesidades.

4. **Validación**:
   - Compila y publica la extensión en Business Central.
   - Prueba los objetos creados (tablas, páginas, validaciones).

5. **Iteración**:
   - Ajusta los ejemplos según los resultados obtenidos.
   - Experimenta con nuevos prompts para ampliar el laboratorio.

## Desde Cero: Crear un Proyecto AL (Versión Simplificada)

1. **Crear el Proyecto AL**:
   - Abre Visual Studio Code.
   - Instala la extensión AL Language desde el Marketplace.
   - Usa el comando `AL: Go!` para generar un nuevo proyecto AL.
   - Configura el archivo `launch.json` para conectarte a tu entorno de Business Central.

2. **Configurar GitHub Copilot**:
   - Asegúrate de que GitHub Copilot esté habilitado en Visual Studio Code.
   - Revisa las configuraciones de Copilot para optimizar la generación de código.

3. **Primer Prompt**:
   - Escribe un prompt como: "Crea una tabla para almacenar puntos de cliente con validación".
   - Observa cómo Copilot genera el código inicial.

4. **Revisión y Ajustes**:
   - Revisa el código generado por Copilot.
   - Ajusta el código según tus necesidades.

5. **Pruebas**:
   - Compila y publica el proyecto en Business Central.
   - Verifica que los objetos creados funcionen correctamente.

6. **Iteración**:
   - Experimenta con nuevos prompts para ampliar el proyecto.

## Notas
- Asegúrate de seguir las reglas de estilo proporcionadas.
- Los ejemplos están diseñados para ser simples y fáciles de entender.

¡Explora y aprende!
