---

mode: 'agent'
tools: ['browser_navigate', 'browser_click']
description: 'Este prompt está diseñado para extraer la clasificación de 2a RFEF utilizando el MCP Server de Playwright.'

---

Navigate to https://www.marca.com/futbol/segunda-rfef/clasificacion/grupo-1.html?intcmp=MENUMIGA&s_kw=clasificacion and extract the clasification of the teams.

For each team, collect and store the following properties in an array of objects:

equipo

Totales PT

Totales PJ

Totales PE

Totales PP

Totales GF

Totales GC


Dump the full array into a single JSON file named clasificacion_2rfef_g1_by_playwright.json inside the MCP-GITHUB-COPILOT/data directory. The file must contain an array of objects, where each element represents a team with the statistics.

IMPORTANT: Teams must appear in the same order as they do on the website. Do not change the teams order. If any property is missing, leave it empty string.

Do not make up any data—only include sessions that you actually retrieve from the Codemotion URL.