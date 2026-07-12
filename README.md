# ⚽ FIFA Torneos

PWA para registrar torneos de FIFA **entre amigos**. Los que compiten son los jugadores; el club (PSG, Real Madrid...) se elige en cada partido. Single-file, sin build step, 100% localStorage.

## Cómo funciona

1. **Jugadores**: agrega a tus amigos (los que compiten en la liga)
2. **Clubes**: catálogo precargado (PSG, Real Madrid, Colo-Colo...) + agrega los tuyos
3. **Torneo**: elige formato y jugadores
4. **Cada partido**: registras quién jugó, con qué club, y el marcador

## Formatos

- **Liga con sorteo**: fixture todos-contra-todos automático (ida o ida/vuelta)
- **Liga libre** ✍️: sin fixture fijo — tú registras cada partido cuando se juega y la tabla se arma sola
- **Eliminatoria**: llaves sorteadas, byes automáticos, penales en empates
- **Grupos + Copa**: estilo Mundial (2 o 4 grupos, clasifican 2, cruces 1A vs 2B)

## Características

- Tabla de posiciones con criterios FIFA (Pts → DG → GF)
- Bracket visual con avance automático
- Marcador tipo estadio con selector de club por lado
- Palmarés e historial de campeones por jugador
- Export/Import JSON para respaldo
- PWA instalable, funciona offline
- **Todos los datos viven en localStorage del navegador** — nada sale de tu dispositivo

## Stack

React 18 UMD + Babel standalone 7 (versiones fijadas) · CSS custom · localStorage (`fifa_tracker_v1`) · Service Worker network-first

## URL

https://angulodev.github.io/FIFA-tracker/
