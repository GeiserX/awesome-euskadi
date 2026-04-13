# AGENTS.md — awesome-euskadi

## Propósito

Selección de software open source que da **soporte específico a Euskadi (País Vasco)** — su gobierno autonómico, diputaciones forales, ayuntamientos, universidades, empresas, infraestructuras y patrimonio. Todo el contenido en español. El foco es Euskadi: el software debe dirigirse específicamente a esta comunidad autónoma o a sus municipios.

## Ámbito

- **3 provincias / territorios históricos**: Araba/Álava, Gipuzkoa/Guipúzcoa, Bizkaia/Vizcaya.
- Principales ciudades: Vitoria-Gasteiz (capital), Bilbao, Donostia-San Sebastián, Barakaldo, Getxo, Irun, Portugalete, Santurtzi, Basauri, Durango.
- **Universidades**: UPV/EHU (Universidad del País Vasco / Euskal Herriko Unibertsitatea), Deusto, Mondragón.
- **Instituciones**: Gobierno Vasco / Eusko Jaurlaritza, Eustat (Instituto Vasco de Estadística), EJIE (Sociedad Informática del Gobierno Vasco), SPRI (Sociedad para la Promoción y Reconversión Industrial), Ikerbasque (Fundación Vasca para la Ciencia), Osakidetza (Servicio Vasco de Salud), Open Data Euskadi.

## Criterios de inclusión

### Incluir

- Software que interactúa con el **Gobierno Vasco** o sus organismos (Open Data Euskadi, Irekia, Udalmap).
- Herramientas para **ayuntamientos** de Euskadi o **diputaciones forales**.
- Software de **universidades vascas** (UPV/EHU, Deusto, Mondragón) cuando sea específico de la región o la universidad.
- Herramientas de **datos abiertos** de Euskadi (opendata.euskadi.eus, Eustat).
- Software de **procesamiento del lenguaje natural** para **euskera** (NLP, TTS, corpus, diccionarios).
- Software de **transporte** vasco (Metro Bilbao, Euskotren, BizkaiBus, Bilbobus).
- Herramientas de **cartografía y SIG** específicas de Euskadi.
- Software sobre **turismo y patrimonio** de la región.
- Proyectos del **sistema sanitario vasco** (Osakidetza).
- Software **educativo** específico de la región.
- Herramientas de **meteorología** regional.
- Proyectos de **industria y empresa** vasca (SPRI, cooperativas, Mondragón).

### No incluir

- Software **genérico** que funciona en toda España sin funcionalidad específica de Euskadi — eso pertenece a awesome-spain.
- Software de **ámbito europeo** — eso pertenece a awesome-europe.
- Software de **otras comunidades autónomas** españolas.
- Software creado por vascos que **no tiene funcionalidad específica** de la región.
- Repositorios **archivados o de solo lectura** — van a `DELETED.md`.
- Repos donde el autor indica que el proyecto está **roto, sin mantenimiento o deprecado**.
- Repos **sin README significativo** o que son claramente repos de test/experimento.
- Ejercicios de clase o trabajos académicos sin utilidad real.

### Zona gris — usar criterio

- Proyectos de universidades vascas que podrían ser genéricos — incluir si tienen datos o configuración específica de Euskadi.
- Software que cubre Euskadi junto con otras regiones — incluir si Euskadi es un foco principal.

## Estándares de calidad

**Mismo listón que [awesome-spain](https://github.com/GeiserX/awesome-spain):**

- **No repos archivados**: si se descubre archivado tras la inclusión, mover a `DELETED.md` inmediatamente.
- **No repos extremadamente sin mantenimiento**: al menos un commit en los últimos 3 años, salvo que sea un proyecto claramente estable/completo.
- **No repos rotos**: si el README dice «deprecated», «no longer maintained», «use X instead» o similar — no incluir. Mover a `DELETED.md` si ya está listado.
- **Estrellas mínimas**: preferir repos con al menos unas pocas estrellas, pero herramientas nicho excepcionales con 0-1 estrellas pueden incluirse si cubren un hueco importante.
- **Verificar cada repo** antes de añadir: comprobar `archived`, `pushed_at`, `stargazers_count` vía `gh api repos/owner/name`.

## Formato de entrada

```markdown
- [Nombre](https://github.com/owner/repo) [![Stars](...)](stargazers) [![Last Commit](...)](commits) [![Language](...)](repo) [![License](...)](LICENSE) [![Tag](...)](url) - Descripción que empieza en mayúscula y termina con punto.
```

Las insignias se generan automáticamente con `scripts/transform-readme.py`. Para contribuir, basta con añadir la entrada en formato simple:

```markdown
- [Nombre](https://github.com/owner/repo) - Descripción que empieza en mayúscula y termina con punto.
```

- La descripción **no debe empezar con el nombre** del proyecto.
- Máximo una línea por entrada.
- Validar con awesome-lint-extra: `python3 lint.py` o mediante el workflow de CI.
- Entradas en **orden alfabético** dentro de cada categoría.
- Categorías en **orden alfabético** en el índice y en el cuerpo del documento.
- Entradas en `DELETED.md` también en **orden alfabético** dentro de cada sección.

## Verificación antes de añadir

Antes de incluir un repositorio, comprobar:

- **Existe y es público**: el enlace de GitHub funciona y el repo no es privado.
- **No está archivado o de solo lectura**: si archivado, va a `DELETED.md` (sección «Archivados»).
- **No está deprecado**: comprobar si el README dice «deprecated», «unmaintained», «broken», «use X instead».
- **Actividad razonable**: al menos un commit en los últimos 3 años, salvo que sea un proyecto estable/completo.
- **No es un duplicado**: cruzar con `README.md` y `DELETED.md`.
- **Calidad mínima**: tiene documentación (README) y no es un repositorio vacío o de test.

## Pull requests y contribuciones

- Las PRs deben usar la plantilla en `.github/PULL_REQUEST_TEMPLATE.md`.
- **Obligatorio**: incluir en la PR la **URL del servicio, API o institución vasca** a la que el software da soporte.
- Plantillas de issues disponibles para sugerir proyectos (`anadir-proyecto.md`) y solicitar retirada (`retirar-proyecto.md`).

## Estructura

- Secciones con `##`, subsecciones con `###`.
- Índice de contenido al principio entre comentarios `<!--lint disable/enable awesome-list-item-->`.
- Al final: sección Contribuir, Nota y Descargo de responsabilidad (como párrafos en negrita, no encabezados ##).

## Temas prohibidos

No se aceptan proyectos relacionados con: pornografía, contenido NSFW, loterías o apuestas, religión, política partidista.

## Difusión

- Notificar a los propietarios de repos abriendo un issue titulado «Listado en awesome-euskadi» con un breve mensaje en español (tuteo) ofreciendo retirar si lo prefieren. Solo 1 issue por organización/usuario — no spamear repos del mismo propietario.
- Publicar en comunidades vascas (Reddit, foros de la UPV/EHU, Telegram de devs vascos) tras alcanzar masa crítica.
- Enviar PR a [sindresorhus/awesome](https://github.com/sindresorhus/awesome) tras 30 días desde la creación del repo.

## Aprendizajes

- Euskadi tiene un ecosistema tech fuerte con instituciones como Eustat, EJIE, Vicomtech, HiTZ y Aholab con presencia en GitHub.
- El centro HiTZ de la UPV/EHU tiene repos de NLP para euskera de gran calidad: Latxa (LLM), Latxa-Instruct, EuskañolDS.
- Aholab (UPV/EHU) desarrolla AhoTTS, un TTS para euskera y castellano con 18★ — el repo con más estrellas de la lista.
- Open Data Euskadi tiene organización `opendata-euskadi` en GitHub con repos de Linked Data, pero la mayoría son de baja actividad.
- Eustat tiene 3 repos oficiales (API-Eustat, eustat.github.io, sdg-data-prod) — todos activos en 2026.
- La búsqueda de EJIE-GV e irekia como organizaciones de GitHub no dio resultados (no existen o son privadas).
- Metro Bilbao tiene `kirisuoc/metrobilbao-now` como herramienta CLI útil.
- Las plantillas LaTeX de la UPV/EHU (EIB_TFG, EIB_TFM, iflatex) son proyectos estables con buenas estrellas.
- BilbaoDynamics/Pinchy es un robot educativo fabricado en Bilbao con 7★.

*Generated by [LynxPrompt](https://lynxprompt.com) CLI*
