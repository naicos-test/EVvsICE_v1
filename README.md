# EV vs ICE — Comparador Económico (TCO/NPV)

Herramienta web 100% estática para comparar económicamente un vehículo eléctrico (EV) versus uno a combustión (ICE) usando:
- NPV del costo total
- Costo anual equivalente (EAC)
- Costo por km (LCO)

## Características
- **Parámetros guardados en la URL** para compartir escenarios (`Compartir escenario`).
- **Tarifas eléctricas**: plana o **TOU** (valle + punta).
- **Gráfico Tornado** (sensibilidades).
- **Gráfico de líneas** con **costos acumulados (valor presente)** por año y **punto de intersección**.
- Exportar **CSV** (Excel) y **PDF**.

## Deploy rápido (GitHub Pages)
1. Crea un repo público, sube `index.html`, `ayuda.html`, `logo.svg` y este `README.md`.
2. `Settings → Pages → Deploy from a branch → main / root`.
3. Abre tu URL: `https://usuario.github.io/ev-vs-ice-tco/`.

## Uso
1. Ajusta supuestos.
2. Click en **Calcular**.
3. **Compartir escenario**: genera un link con todos los parámetros.
4. **Exportar CSV/PDF** según necesites.

## Estructura
- `index.html`: App principal.
- `ayuda.html`: Explicaciones y notas.
- `logo.svg`: Logo.
- `README.md`: Este archivo.

## Notas
- Los resultados dependen de los supuestos. Ajusta: km/año, energía, mantenciones, residuales, tasa y horizonte.
- El **gráfico de costos** usa **valor presente** por año (descuento con r).
- El **punto de intersección** se aproxima por el año donde las curvas se cruzan (o el más cercano).

## Licencia
MIT
