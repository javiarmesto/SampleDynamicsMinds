# SampleDynamicsMinds · BizzApps4all

Ejemplo mínimo AL: la pageextension **50200 CustomerListExt** amplía **Customer List** y muestra `App published: Hello world` al abrirla. El código está en [HelloWorld.al](HelloWorld.al).

## Requisitos y estado

[app.json](app.json) declara BizzApps4all 1.0.0.0, application **28.0.0.0**, runtime **17.0** y rango 50200–50249. Necesitas VS Code con AL Language y un sandbox compatible, con permiso para publicar extensiones. Es una demostración para DynamicsMinds; no es la distribución de ALDC. Las carpetas `.github/` y `.agents/` conservan material de desarrollo asistido.

## Inicio rápido

```powershell
git clone https://github.com/javiarmesto/SampleDynamicsMinds.git
cd SampleDynamicsMinds
code .
```

Configura `.vscode/launch.json` con tu tenant y sandbox, sin reutilizar valores personales del checkout. Ejecuta **AL: Download Symbols**, compila con `Ctrl+Shift+B` y publica con `F5`. Abre **Clientes / Customer List**: el resultado esperado es el mensaje anterior. No se requiere Azure OpenAI ni una llamada MCP para ese comportamiento.

## Estructura y límites

- `HelloWorld.al`: único objeto funcional del ejemplo.
- `app.json`: versión, runtime e IDs.
- `.vscode/`: ajustes del entorno; revísalos antes de usarlos.
- `.alpackages/`: símbolos versionados del ejemplo; no prueban compatibilidad con tu sandbox. Descarga los tuyos.
- `.github/`, `.agents/`, `apm.yml`, `aldc.yaml`: contexto de herramientas, separado de la función Hello World.

GitHub prioriza `.github/README.md`; esa portada también describe este ejemplo. La anterior portada copiada de ALDC anunciaba una licencia de otro proyecto: no se ha confirmado una licencia que cubra BizzApps4all. No se asigna una licencia nueva en esta revisión.

Inspección estática: **6 de octubre de 2026**. La compilación, publicación y apertura de la página quedan por comprobar en tu sandbox. Para informar de un problema, incluye versión BC, comando y error sin credenciales. [ALDC canónico](https://github.com/javiarmesto/ALDC-AL-Development-Collection).
