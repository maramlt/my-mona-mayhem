# 🎮 Mona Mayhem — Taller de GitHub Copilot

---

> **Duración:** ~1 hora  
> **Nivel:** Intermedio  
> **Pila tecnológica:** Astro / Node.js / TypeScript

Construye una aplicación retro de estilo arcade para comparar contribuciones de GitHub — **Mona Mayhem** — mientras aprendes a utilizar toda la gama de flujos de trabajo de GitHub Copilot. El taller ofrece **dos itinerarios**: uno con VS Code y otro con GitHub Copilot CLI.

---

## 🎯 Elige tu itinerario

- **Itinerario de VS Code** — trabaja desde el editor y practica Chat, Plan Mode, Agent Mode, los agentes en segundo plano y el ciclo de revisión integrado.
- **Itinerario del CLI** — trabaja desde el terminal y practica `copilot`, el contexto con `@file`, `/plan`, las ediciones autónomas, `/fleet`, `/delegate` y `/review`.

Sigue la pista que coincida con tu flujo de trabajo preferido.

---

## 📋 Lista de Verificación Rápida

Antes de empezar, verifica:

- [ ] GitHub Copilot está habilitado para tu cuenta
- [ ] Node.js está instalado
- [ ] Git está instalado y configurado
- [ ] El navegador y el terminal están listos

<!-- track:vscode:start -->
- [ ] VS Code **v1.107+** (sin actualizaciones pendientes)
- [ ] Has iniciado sesión en la extensión **GitHub Copilot**
- [ ] El panel de Chat está abierto y Agent está listo
<!-- track:vscode:end -->

<!-- track:cli:start -->
- [ ] GitHub Copilot CLI instalado y disponible como `copilot`
- [ ] Has iniciado sesión en el CLI con `/login`
- [ ] Te manejas con comandos slash como `/help`, `/plan` y `/review`
<!-- track:cli:end -->

> 💡 **Consejo:** Usa el DevContainer para disponer de un entorno preconfigurado y empezar rápidamente en VS Code.

---

## 🧠 Lo Que Aprenderás

| # | Habilidad | Descripción |
|---|-----------|-------------|
| 1 | **Ingeniería de contexto** | Enseñar a Copilot cómo es tu código base con instrucciones, referencias y restricciones claras |
| 2 | **Planificar primero** | Diseñar la arquitectura antes de implementar |
| 3 | **Implementación agéntica** | Supervisar a Copilot mientras realiza tareas de programación en varios pasos |
| 4 | **Diseño iterativo** | Usar Copilot para transformar el aspecto visual y perfeccionar los detalles de interacción |
| 5 | **Flujos de trabajo en paralelo** | Repartir el trabajo entre agentes, sesiones o tareas delegadas |

<!-- track:vscode:start -->
### Funcionalidades de VS Code

- **Chat + modo Ask** para explorar
- **Plan Mode** para prompts de arquitectura y diseño
- **Agent Mode** para implementación en múltiples archivos
- **Agentes en segundo plano y en la nube** para pulido en paralelo
<!-- track:vscode:end -->

<!-- track:cli:start -->
### Funcionalidades de Copilot CLI

- **Sesiones interactivas del CLI** con `copilot`
- **`/plan` y Shift+Tab** para planificación estructurada
- **Ediciones autónomas** con aprobaciones en línea y `/diff`
- **`/fleet`, `/delegate` y `/review`** para paralelismo y controles de calidad
<!-- track:cli:end -->

---

## 📚 Partes del Laboratorio

| Parte | Título | Descripción |
|-------|--------|-------------|
| [**01**](01-setup.md) | Configuración e ingeniería de contexto | Crea tu repositorio, prepara el entorno y proporciona a Copilot el contexto adecuado |
| [**02**](02-plan-and-scaffold.md) | Planificación y estructura inicial | Diseña la API y la arquitectura de la página antes de implementar |
| [**03**](03-agent-mode.md) | Construcción del juego | Conecta la página de batalla y los gráficos de contribuciones con ayuda agéntica |
| [**04**](04-design-vibes.md) | Tematización orientada al diseño | Convierte la estructura inicial en una experiencia de arcade retro |
| [**05**](05-polish.md) | Pulido y trabajo en paralelo | Usa flujos de trabajo con varios agentes para mejorar la experiencia, la resiliencia y la calidad |
| [**06**](06-bonus.md) | Bonus y ampliaciones | Explora ideas de funcionalidades, formas de compartir y experimentos adicionales |

---

## 💡 Consejos Pro

1. **Mantén el navegador abierto** — observa los cambios en tiempo real mientras programas.
2. **Haz commits con frecuencia** — guarda puntos de control limpios mientras iteras.
3. **Perfecciona el plan antes de implementar** — los mejores planes dan mejores resultados.
4. **Revisa los cambios de Copilot** — usa la vista de diferencias o las herramientas de revisión del CLI en lugar de aceptarlos sin comprobarlos.

<!-- track:vscode:start -->
5. **Usa los puntos de control y Deshacer** en el chat si una iteración se desvía.
<!-- track:vscode:end -->

<!-- track:cli:start -->
5. **Usa `/session`, `/context` y `/share file`** cuando quieras inspeccionar o guardar tu trabajo.
<!-- track:cli:end -->
