<!-- l10n-sync: source-file="workshop/06-bonus.md" -->
# 🎉 Bonus y ampliaciones

---

¡Has creado una aplicación de GitHub Battle completamente funcional! Ahora es el momento de ir más allá con **desafíos abiertos**.

<!-- track:vscode:start -->
Usa **Agent Mode** para todos estos desafíos: describe lo que quieres y deja que Copilot te ayude a implementarlo.
<!-- track:vscode:end -->

<!-- track:cli:start -->
Usa Copilot CLI para todos estos desafíos: combina el contexto con `@file`, `/plan`, el modo normal y `/review` según sea necesario.
<!-- track:cli:end -->

---

## 🏆 Desafío 1: Anuncio del ganador

Cuando se hayan cargado los dos gráficos de contribuciones, compara los totales y muestra un anuncio dinámico del ganador.

**Qué construir:**
- Compara el total de contribuciones de ambos usuarios.
- Muestra **"🏆 {username} WINS! 🏆"** con un estilo festivo si hay un ganador claro.
- Muestra **"🤝 IT'S A TIE! 🤝"** si ambos tienen el mismo número de contribuciones.
- Añade una animación o confeti para darle más vistosidad.

**Sugerencia de prompt:**
> Cuando se hayan cargado los datos de contribuciones de ambos usuarios, compara los totales y muestra un anuncio del ganador. Muestra «🏆 {username} WINS! 🏆» si un usuario tiene más contribuciones, o «🤝 IT'S A TIE! 🤝» si tienen el mismo número. Dale un aspecto llamativo con animaciones CSS.

---

## 🏆 Desafío 2: Contador de rachas

Calcula y muestra la racha más larga de días consecutivos con contribuciones de cada usuario.

**Qué construir:**
- Analiza día a día los datos de contribuciones.
- Encuentra la serie más larga de días consecutivos con al menos una contribución.
- Muestra de forma destacada la duración de la racha de cada usuario.
- Resalta quién tiene la racha más larga.

**Sugerencia de prompt:**
> Añade un contador de rachas que analice los datos de contribuciones de cada usuario para encontrar su racha más larga de días consecutivos. Debajo del gráfico de contribuciones de cada usuario, muestra «🔥 Longest Streak: X days».

---

## 🏆 Desafío 3: Historial de batallas

Guarda los resultados de las batallas para que se puedan consultar los enfrentamientos anteriores.

**Qué construir:**
- Guarda en `localStorage` el resultado de cada batalla (nombres de usuario, totales, ganador y marca de tiempo).
- Añade una sección **"Recent Battles"** debajo del área principal de batalla.
- Muestra los resultados de las últimas 5–10 batallas.
- Añade un botón «Clear History».

**Sugerencia de prompt:**
> Guarda los resultados de cada batalla en localStorage después de compararlos. Añade una sección «Recent Battles» que muestre las últimas 10 batallas, los nombres de usuario, el total de contribuciones, el ganador y la fecha de cada batalla. Incluye un botón «Clear History».

---

## 🏆 Desafío 4: Efectos de sonido

Añade efectos de sonido de arcade retro con la Web Audio API, sin necesidad de archivos externos.

**Qué construir:**
- Un sonido de **inserción de moneda** al hacer clic en el botón «Battle!».
- Un sonido de **potenciación** cuando se carguen correctamente los resultados.
- Un sonido de **explosión** cuando se produzca un error (usuario no encontrado o fallo de la API).
- Un botón para activar o silenciar el sonido.

**Sugerencia de prompt:**
> Añade efectos de sonido de arcade retro con la Web Audio API (sin archivos de audio). Reproduce el sonido de insertar una moneda al iniciar una batalla, el de potenciación cuando se carguen los resultados y el de explosión cuando se produzca un error. Genera los sonidos mediante código con osciladores y nodos de ganancia. Incluye un control para silenciar el sonido.

---

## 🏆 Desafío 5: Secuencia de batalla animada

Crea expectación con una cuenta atrás dramática antes de mostrar los resultados.

**Qué construir:**
- Al hacer clic en «Battle!», muestra una superposición a pantalla completa.
- Anima la secuencia: **"3..."** → **"2..."** → **"1..."** → **"⚡ FIGHT! ⚡"**.
- Después, muestra los gráficos de contribuciones con una entrada espectacular.
- Usa animaciones CSS o temporizadores de JavaScript.

**Sugerencia de prompt:**
> Añade una secuencia de batalla animada al hacer clic en «Battle!». Muestra una cuenta atrás superpuesta: «3...», «2...», «1...» y «⚡ FIGHT! ⚡», con una duración aproximada de 1 segundo por paso. Cuando termine la cuenta atrás, muestra los resultados con una animación de entrada lateral.

---

## 🏆 Desafío 6: Leyenda de contribuciones

Añade una leyenda de escala de colores que coincida con la paleta del gráfico de contribuciones.

**Qué construir:**
- Una leyenda horizontal con los niveles de intensidad de las contribuciones.
- Etiquetas desde **"Less"** hasta **"More"**.
- La paleta de colores real de la respuesta de la API de contribuciones de GitHub.
- Colócala cerca de los gráficos de contribuciones.

**Sugerencia de prompt:**
> Añade debajo de los gráficos una leyenda de contribuciones que muestre la escala de colores de la paleta de la API. Muestra una fila de cuadrados de color desde «Less» (el más claro) hasta «More» (el más oscuro), según los colores reales de los niveles de contribución que devuelve la API.

---

## 🏆 Desafío 7: Compartir resultados

Permite compartir los resultados de una batalla con un solo clic.

**Qué construir:**
- Un botón **"📋 Share Results"** que aparece después de una batalla.
- Copia al portapapeles un resumen de texto con formato.
- Incluye los nombres de usuario, los totales de contribuciones y el ganador.
- Muestra brevemente el mensaje de confirmación «Copied!».

**Sugerencia de prompt:**
> Añade un botón «📋 Share Results» que copie al portapapeles un resumen de la batalla con formato. El resumen debe incluir ambos nombres de usuario, sus totales de contribuciones y quién ha ganado. Usa la Clipboard API y muestra brevemente el mensaje «Copied to clipboard!» para confirmar la copia.

---

<!-- track:cli:start -->
## 💻 Extras del CLI

Si quieres explorar más funcionalidades de Copilot CLI después del taller principal:

- Usa `copilot -p "Write a conventional commit message for the current git diff"` para generar una respuesta rápida de un solo disparo que puedes pegar en Git.
- Ejecuta `/share file` para guardar tu sesión como Markdown para referencia futura.
- Usa `/session` y `/session plan` para inspeccionar cómo el CLI está rastreando tu trabajo actual.
<!-- track:cli:end -->

## 🎊 ¡Enhorabuena!

¡Has completado el taller **Mona Mayhem: GitHub Battle**! Esto es lo que has conseguido:

### Lo que has creado

- ✅ Una **aplicación web multipágina completa** a partir de una especificación de diseño.
- ✅ Una **página de inicio** con temática de arcade retro y diseño adaptable.
- ✅ Una **arena de batalla** que obtiene y compara datos reales de contribuciones de GitHub.
- ✅ **Gráficos de contribuciones interactivos** con niveles de actividad diferenciados por colores.
- ✅ **Gestión de errores, estados de carga y mejoras de accesibilidad**.
- ✅ **Diseño adaptable** para distintos dispositivos.

### Lo que has practicado

| Habilidad | Lo Que Practicaste |
|-----------|-------------------|
| **Ingeniería de contexto** | Proporcionar a Copilot los archivos, las instrucciones y las restricciones adecuadas |
| **Planificación** | Generar y perfeccionar planes de implementación antes de programar |
| **Programación agéntica** | Delegar en Copilot tareas de varios pasos que afectan a distintos archivos |
| **Iteración del diseño** | Partir de una dirección visual y perfeccionarla hasta obtener un resultado pulido |
| **Disciplina de revisión** | Inspeccionar los cambios generados por IA antes de hacer commit |

### 🚀 Sigue aprendiendo

- 📺 [Canal de YouTube de VS Code](https://www.youtube.com/@code) — Tips, tutoriales y novedades
- 📖 [Documentación de GitHub Copilot](https://docs.github.com/en/copilot) — Documentación oficial y guías
- 💻 [Documentación de GitHub Copilot CLI](https://docs.github.com/en/copilot/how-tos/copilot-cli) — Instalación, comandos slash y mejores prácticas
- 🌟 [Awesome GitHub Copilot](https://github.com/stefanprodan/awesome-github-copilot) — Recursos y ejemplos de la comunidad
- 🛠️ [Talleres de Copilot Dev Days](https://github.com/github/copilot-dev-days) — Más talleres prácticos como este

---

## 🙏 ¡Gracias!

¡Gracias por participar en este taller! Has descubierto cómo GitHub Copilot puede acelerar todas las fases del desarrollo, desde la planificación y el diseño hasta la implementación y el pulido. Las técnicas que has practicado aquí sirven para cualquier proyecto, framework y escala. ¡Ahora ve y crea algo increíble! 🚀
