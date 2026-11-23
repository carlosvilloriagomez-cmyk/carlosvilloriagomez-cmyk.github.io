# Proyecto: web personal + videocurrículum de Carlos Villoria Gómez

Web estática en GitHub Pages. Repo: `carlosvilloriagomez-cmyk/carlosvilloriagomez-cmyk.github.io`
URL pública: https://carlosvilloriagomez-cmyk.github.io/

## Reglas que no se pueden romper
- **La URL no puede cambiar.** Hay tarjetas de visita impresas con esa URL y un QR. No renombrar el repo, no cambiar de usuario, no mover `index.html` fuera de la raíz.
- Sitio 100 % estático: HTML, CSS y JS sin build obligatorio. Debe funcionar en GitHub Pages tal cual (rama `main`, carpeta raíz).
- Se abre sobre todo desde el móvil escaneando el QR. Mobile first, carga rápida, animaciones ligeras, respetar `prefers-reduced-motion`.
- Añadir contenido (fotos, vídeos, PDFs) no debe obligar a tocar la estructura: se sueltan archivos en `assets/` con los nombres que usa el HTML.
- Idioma: español de España. No inventar datos: usar solo lo que hay en este documento.
- Limite de GitHub: archivos de más de 100 MB no se pueden subir. Los vídeos pesados van en YouTube (no listado) y se incrustan con el atributo `data-yt`.

## Estilo (debe coincidir con la tarjeta de visita impresa)
Oscuro, estética de periodismo de datos / think tank joven.
- Fondo `#0F172A` con cuadrícula tenue (líneas de 1 px a ~7 % de opacidad cada 44 px).
- Barra roja vertical fija en el borde izquierdo (14 px, 10 px en móvil), `#E11D48`.
- Rojo `#E11D48` (texto pequeño: `#FB7185`), azul `#0284C7` (texto pequeño: `#7DD3FC`).
- Paneles `#131D35`, bordes `#1F2A44`, texto `#CBD5E1`, títulos `#F1F5F9`, apagado `#94A3B8`.
- Fuentes (Google Fonts): **Space Grotesk** 700 para títulos, **IBM Plex Sans** para texto, **IBM Plex Mono** en mayúsculas con tracking para etiquetas.
- Elementos de marca: etiqueta roja "VÍDEO CURRÍCULUM", nombre en dos líneas (Carlos Villoria en blanco, "Gómez" en rojo), foto con bloque rojo desplazado detrás, líneas de gráfico azul y roja con área roja translúcida y punto marcado con anillo, numeración de secciones en cajitas rojas.
- La web actual (`index.html`) ya implementa esto. Sirve de base; se puede rehacer entera si mejora el resultado.

## Lo que se quiere ahora
Un acabado muy profesional con animaciones: aparición de secciones al hacer scroll, barridos de color en títulos, líneas de gráfico que se dibujan, contadores, línea de tiempo con progreso, parallax suave. Se permite GSAP desde CDN. Nada que dañe el rendimiento en móvil. El videocurrículum debe seguir siendo lo primero que ve el visitante.
- **Sin scroll suavizado (Lenis):** se probó y en PC con touchpad se notaba retardado. Scroll nativo en todos los dispositivos.
- **Todo el contenido debe verse aunque falle JavaScript o el CDN.** Las animaciones solo mejoran, nunca ocultan.

## Estructura de la web (orden decidido con Carlos)
1. Cabecera: nombre, entradilla, chips, foto de perfil (`foto-perfil.jpg`), gráfico decorativo.
2. **Videocurrículum** (vídeo grande, lo primero tras la cabecera; hasta que exista el nuevo muestra "Próximamente").
3. **Yo**: biografía e intereses.
4. **Estudios**: Universidad de Málaga, certificado de inglés B2 (`ingles-b2.jpg`), diplomas. Foto informal `foto-estudios.jpg` (la del mar, encaja con "venirme a conocer mundo").
5. **Concurso Generación €uro**: foto del equipo, diploma, tres páginas del trabajo.
6. **Experiencia**: Talent Land 2026.
7. **Proyectos con IA**: primer videocurrículum junto al actual, anuncio, memoria del prompt, n8n, material didáctico. Foto relajada y tecnológica `foto-proyectos.jpg`.
8. **Contacto**: email, teléfono, y LinkedIn/Instagram si se añaden.

Las fotos personales se reparten por la página (cabecera, Yo, estudios, proyectos), no solo una. La de la cabecera es provisional: Carlos puede sustituirla por una nueva con traje y la cara visible. En "Yo" hay un hueco para `assets/img/foto-yo.jpg` (vertical 4:5, distinta a las demás), pendiente de que Carlos la elija.

## Contenido (fuente de verdad)
**Datos:** Carlos Villoria Gómez, 19 años, nacido en Salamanca, vive en Málaga. Email carlos.villoria.gomez@gmail.com, teléfono +34 622 76 29 86.

**Biografía:** joven atrevido, auténtico y exigente; lo demuestra habiéndose ido a vivir solo a Málaga sin conocer a nadie, para conocer mundo, ser más independiente y buscar oportunidades lejos de su ciudad natal. Intereses: economía, geopolítica, filosofía, IA, psicología. Sigue canales como Memorias de Pez y Solo Fonseca; tiene cuadernos de NotebookLM (p. ej. sobre el sistema J-Alert de Japón). Ningún proyecto grande de economía/geopolítica aparte del concurso.

**Lecturas:** *El hombre en busca de sentido* (Viktor Frankl), *El manantial* (Ayn Rand) y *La economía en una lección* (Henry Hazlitt) son sus favoritos. También ha leído *Así habló Zaratustra* (Nietzsche), *Diarios del opio* (David Jiménez) y *Memorias de Adriano* (Marguerite Yourcenar).

**Qué busca:** no solo marketing y contenido con IA. También le encantaría trabajar como analista de datos geopolíticos, redactor de guiones para vídeos de geopolítica o investigador de fuentes. No describirlo como si solo buscara prácticas de marketing.

**IA:** usa Gemini, NotebookLM, ChatGPT y Claude. Experiencia mínima en vídeo hiperrealista: proyecto pospuesto por necesitar herramientas caras (Higgsfield, claves de API). Tiene certificados de la UMA en Ingeniería de Prompts con Gemini y NotebookLM, y en Análisis de Datos con Python. Ha creado vídeos animados con Claude (como el propio videocurrículum) y material didáctico para su padre, maestro de primaria; dice que siempre sienta bien echar una mano a quien te ha dado tanto, pero que necesita un reto mucho mayor que diseñar fichas y exámenes. Bases de automatización con n8n: una automatización sencilla que responde correos automáticamente al detectar palabras clave. En Proyectos se muestra el primer videocurrículum (menos trabajado) junto al actual para destacar la evolución, además del anuncio con IA y la memoria del prompt.

**Memoria del prompt = proyecto "Arquitecto de Asistentes"** (`assets/docs/memoria-prompt.pdf`). **No tiene nada que ver con el anuncio Ocean Shield.** Es un Proyecto de Claude que diseñó para crear nuevos asistentes (agentes). Arquitectura modular de tres piezas: `Project_Instructions.md` (motor en cuatro fases, con invariantes blindados), `Knowledge_Base_Prompting.md` (metodologías de Anthropic, OpenAI, Google, Self-Refine, LLM-as-a-Judge) y `Prompt_Evaluador.md` (auditor externo "critique-first, score-second", que se guarda fuera del proyecto para evitar sesgos). Auditorías en conversaciones limpias: el primer borrador sacó un 73 % y la versión final un 92,5 %.

**Concurso Generación €uro, 13.ª edición (2023-2024):** parte del equipo ganador, IES Fray Luis de León (Salamanca). Analizaron geopolítica e inflación (decisión de política monetaria del Consejo de Gobierno del BCE, 6 de marzo de 2024). Carlos presentó y defendió el análisis frente al jurado, pero el trabajo fue de todo el equipo: no decir que fue "el orador" ni que lo hizo él solo. Diploma de ganador, Banco de España, Madrid, 5 de abril de 2024. Destacar el prestigio y la dificultad del concurso. En las cifras, destacar "1.º" y poner en texto discreto "en la 13.ª edición del Concurso Generación €uro".

**Talent Land Málaga 2026:** asistente de los speakers.

**Estudios:** Grado en Marketing e Investigación de Mercados, Universidad de Málaga, 2.º curso, ninguna asignatura suspensa. Notas destacadas en Análisis Económico, Comportamiento del Consumidor, Gestión del Producto y Branding, Historia del Comercio y Matemáticas para la Economía y la Empresa.

**Diplomas** (Ingeniería de Prompts y Gemini son **el mismo** diploma):
- *Ingeniería de Prompts y gestión del conocimiento con IA generativa: Gemini y NotebookLM para el ámbito académico*, Universidad de Málaga (FGUMA), 25 h online, 1 ECTS, del 15/01/2026 al 16/06/2026, expedido el 29/06/2026. Imagen: `assets/img/diploma-prompts.jpg`.
- *Análisis de Datos con Python*, Universidad de Málaga (FGUMA), 25 h (10 presenciales y 15 online), 1 ECTS, del 17 al 22/11/2025, expedido el 17/12/2025. Programa: Python, Jupyter, POO, minería de datos, aprendizaje automático, NumPy, SciPy, Pandas, Matplotlib, Scikit-learn. Imagen: `assets/img/diploma-python.jpg`.
- Las imágenes de los diplomas de la UMA tienen el **DNI tapado** y están recortadas sin el bloque de verificación (código CSV, URL y QR), porque esa verificación muestra el original con el DNI. Los PDF originales no se suben al repo.
- Acreditación de inglés (imagen `assets/img/ingles-b2.jpg`): B2 CEFR en el 360°LPT de Capman Testing Solutions, puntuación global 293 (Listening 81, Reading 74, Speaking 71, Writing 67), 18/02/2026.

## Archivos y huecos de contenido
`index.html` carga todo desde `assets/`. Si un archivo no existe se muestra "Próximamente".
- Fotos personales (listas): `foto-perfil.jpg` (cabecera), `foto-estudios.jpg`, `foto-proyectos.jpg`.
- `assets/img/ingles-b2.jpg`: certificado de inglés (Capman 360°LPT, nivel B2 CEFR, 293 puntos, 18/02/2026), con DNI y número de referencia tapados. Se dejó el QR de verificación.
- Concurso (listas): `euro-equipo.jpg`, `euro-diploma.jpg`, `euro-instagram.jpg`, `euro-trabajo-portada.jpg`, `euro-trabajo-inflacion.jpg`, `euro-trabajo-previsiones.jpg`.
- Pendientes: `talentland.jpg`, `videocv-poster.jpg`.
- Fotos descartadas de la web (interiores de casa, baño o cara tapada por el móvil): selfies de espejo con camisa negra, sudadera gris y traje gris.
- Vídeos (ya en `assets/videos/`, comprimidos para web con faststart):
  - `videocv-v1.mp4`: **PRIMER videocurrículum** (el menos trabajado), 79 s, vertical 9:16, 720×1280, 4,3 MB. Poster `assets/img/videocv-v1-poster.jpg`. Va en la sección Proyectos para mostrar la evolución.
  - `anuncio.mp4`: anuncio "Ocean Shield", 14 s, vertical 9:16, 720×1280, 3,3 MB. Poster `assets/img/anuncio-poster.jpg`. Va en Proyectos.
  - `videocv.mp4`: **el videocurrículum nuevo y definitivo. Todavía NO existe.** Carlos lo hará después de terminar la web (orden acordado: primero web, luego vídeo). Mientras tanto el hueco principal muestra "Próximamente". Cuando exista: guardarlo como `assets/videos/videocv.mp4` (y su poster `assets/img/videocv-poster.jpg`, añadiendo `data-poster` al bloque) y no hará falta tocar nada más.
  - **Los vídeos son verticales (9:16).** Mostrarlos con `object-fit: contain`, ancho máximo ~340-380 px y altura máxima ~80 vh; nunca recortados a 16:9. En escritorio, texto al lado; en móvil, a ancho completo.
- El primer videocurrículum (v1) usa una paleta distinta (negro con naranja). El nuevo se hará con la paleta de marca roja y azul. El v1 se hizo con Remotion (vídeo programado en React) desde Claude, con subtítulos animados, formato 1080×1920: el nuevo puede hacerse igual.
- Contenido del v1 (no contradecirlo en la web): se presenta como candidato a prácticas en marketing digital y contenido con IA; menciona el Grado en Marketing e Investigación de Mercados (UMA), el anuncio Ocean Shield (4 planos, mismo personaje, creado con ChatGPT y animado con IA), que el propio vídeo se hizo con Claude, el concurso Generación €uro (1.º de unos 2.000 centros, equipo ganador de 4 estudiantes, 13.ª edición, inflación y geopolítica) y análisis de datos con Python (Pandas, NumPy, Matplotlib; certificación de la UMA de dic. 2025, 25 horas). Pendiente de que Carlos confirme las cifras de "unos 2.000 centros" y la certificación de Python.
- PDFs: `assets/docs/memoria-prompt.pdf` (memoria del Arquitecto de Asistentes, ya subida). Los diplomas se muestran como imágenes (ver "Diplomas").
- Si falta algún archivo, el diseño no debe verse roto.

## Privacidad (decisiones tomadas)
- La portada del trabajo tiene tapados los nombres de los compañeros y del tutor. No destaparlos sin que Carlos lo diga.
- La captura de la historia de Instagram está recortada para no mostrar usuarios de terceros.
- La foto del equipo incluye a otras personas: pendiente de que Carlos confirme que están de acuerdo; si es foto oficial del Banco de España, añadir crédito.

## Pendiente de decidir con Carlos
1. ¿Se quita la captura de Instagram (repite el diploma)?
2. ¿Se muestran las tres páginas del trabajo o solo portada y una de gráficas?
3. ¿Se dejan tapados los nombres de la portada?
4. Confirmar la cifra del v1 "unos 2.000 centros" (no ponerla en la web hasta entonces). La certificación de Python de la UMA (dic. 2025, 25 h) ya está confirmada por el diploma.
5. Enlaces de LinkedIn e Instagram (de momento vacíos en el bloque `CFG` al final de `index.html`).
6. Foto para la sección "Yo" (`assets/img/foto-yo.jpg`).

## Cómo trabajar
- Previsualizar en local con `python3 -m http.server` y comprobar en móvil (ancho 390 px) y escritorio.
- Antes de cada `git push`, revisar que `index.html` sigue en la raíz y que no se ha cambiado nada que afecte a la URL.
- Mensajes de commit claros, en español.
