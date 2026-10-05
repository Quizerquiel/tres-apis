# tres-apis

Tres sistemas pequeños hechos con HTML, CSS y JavaScript puro. No usan backend, build ni API keys.

| Carpeta | Qué es | API |
|---|---|---|
| `casa-de-cambio/` | Una casa de cambio de barrio: tablero de tasas, ventanilla que imprime un ticket y una gráfica de 90 días que te dice si conviene cambiar hoy. | [Frankfurter](https://frankfurter.dev) |
| `pasaporte/` | Juego de adivinar países con pistas de un agente de migración. Mientras menos pistas uses, más puntos ganas y más sellos juntas en tu pasaporte. | Datos de [REST Countries](https://restcountries.com) (dataset abierto [mledoze/countries](https://github.com/mledoze/countries)) + banderas de [flagcdn](https://flagcdn.com) |
| `sismografo/` | Estación sismográfica: los sismos reales se dibujan en una tira de papel, con bitácora y un "mapa sin mapa" donde los puntos solos dibujan las placas tectónicas. | [USGS Earthquake feeds](https://earthquake.usgs.gov/earthquakes/feed/v1.0/geojson.php) |

## Correr en local

```bash
npx http-server -p 8080 -c-1
```

Luego abre http://localhost:8080. También funciona `python -m http.server 8080`.

> Nota: la API pública de REST Countries (v1 a v4) fue dada de baja y la v5 pide API key. Por eso el pasaporte lee el mismo dataset abierto en el que se basa REST Countries, servido por jsDelivr.
