<!-- l10n-sync: source-file="workshop/04-design-vibes.md" -->
# Parte 4: Tematización orientada al diseño

---

En esta parte, usarás los ciclos de planificación e implementación de Copilot para diseñar una transformación completa del tema. Este es un desarrollo orientado al diseño: empieza por la visión, itera sobre los elementos visuales y deja que Copilot se encargue del trabajo pesado de CSS.

## Tarea 1: Planifica el tema retro

<!-- track:vscode:start -->
Cambia al modo **Plan** en GitHub Copilot Chat.
<!-- track:vscode:end -->

<!-- track:cli:start -->
Usa `/plan` en GitHub Copilot CLI o pulsa **Shift+Tab** hasta activar el modo plan.
<!-- track:cli:end -->

Escribe este prompt:

> Quiero convertir esta página en una experiencia completa de arcade retro. Planifica una renovación visual integral que incluya: efectos de líneas de barrido CRT en el fondo, un brillo de neón en el título que pulse como un rótulo luminoso, una insignia VS animada con cambios de color en degradado, una capa brillante y reluciente sobre las tarjetas de resultados de los usuarios, animaciones de entrada flotante para los campos de texto, texto de carga que alterne entre verde y morado, y efectos de brillo al pasar el cursor sobre los cuadrados de contribuciones. Mantén el fondo oscuro (`#0a0a1a`) y usa el verde (`#5fed83`) y el morado (`#8a2be2`) como colores de acento. Aplica un tema oscuro con la fuente retro de videojuegos Press Start 2P de Google Fonts.

Copilot generará un plan detallado de implementación con todos los efectos visuales. **No lo aceptes de inmediato**: revísalo e itera:

- Sugiere ajustes en la duración de las animaciones (por ejemplo: «Haz que el pulso de neón sea más lento, de unos 3 segundos»).
- Pregunta por efectos concretos (por ejemplo: «¿Cómo funcionará la capa brillante de las tarjetas?»).
- Pide que cambie el enfoque si algo no te convence.

## Tarea 2: Implementa el tema

Cuando estés conforme con el plan, pide a Copilot que lo implemente.

> Implementa el plan de tema de arcade retro que acabamos de diseñar.

Copilot añadirá varias animaciones CSS, pseudoelementos y transiciones en la hoja de estilos. Por ejemplo, puede incluir:

- `@keyframes` para las líneas de barrido, el pulso de neón, el brillo y los efectos de entrada flotante.
- Pseudoelementos (`::before`, `::after`) para crear efectos superpuestos.
- Propiedades personalizadas de CSS para los colores del tema.
- Transiciones y estados al pasar el cursor para los elementos interactivos.

<!-- track:cli:start -->
Cuando se apliquen los cambios, usa `/diff` para revisar los cambios de estilo antes de aprobarlos.
<!-- track:cli:end -->

## Tarea 3: Perfecciona el ambiente visual

> **⚠️ ¿No ves los cambios?** Si el nuevo tema o las animaciones no aparecen, detén el servidor de desarrollo (`Ctrl+C`), reinícialo con `npm run dev` y fuerza la recarga del navegador (`Ctrl+Shift+R`).

Mantén abierta la vista previa del navegador e itera sobre el diseño. Prueba prompts como estos:

> El efecto de líneas de barrido es demasiado intenso; reduce la opacidad a 0.03.

> Añade un ligero parpadeo eléctrico al texto del título.

> La insignia VS debería pulsar con más intensidad.

Este es un **desarrollo orientado al diseño**: iteras sobre el resultado visual en tiempo real. Cada prompt perfecciona la experiencia hasta que te convenza. No te conformes con algo «aceptable»: lleva el ambiente visual al límite para que la página parezca la de una máquina recreativa.

## Tarea 4: Actualiza las instrucciones

Las instrucciones deben reflejar las decisiones de diseño importantes para que los prompts posteriores mantengan la coherencia.

<!-- track:vscode:start -->
Pide a Copilot Chat:

> Añade a `copilot-instructions.md` una sección de guía de diseño que describa nuestro tema de arcade retro: colores, fuentes y estilo de animación.
<!-- track:vscode:end -->

<!-- track:cli:start -->
Pide a Copilot CLI:

> Actualiza las instrucciones del repositorio con una breve guía de diseño del tema de arcade retro: colores, fuentes, estilo de animación y la regla de que las nuevas interfaces deben mantener la estética de neón.
<!-- track:cli:end -->

Cuando la página tenga el aspecto esperado, haz commit de las instrucciones y los cambios de diseño.

```bash
git add -A
git commit -m "Add retro arcade theme with CRT and neon effects"
git push
```

## ✅ Parte 4 completada

**Lo que has aprendido:**

- Usar flujos de planificación para esbozar un **sistema de diseño antes de implementarlo**.
- **Iterar sobre el resultado visual** con prompts de seguimiento rápidos.
- **Actualizar las instrucciones después de tomar decisiones importantes** para que Copilot mantenga la identidad visual.
