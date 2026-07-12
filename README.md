# ⚽ FIFA Torneos

PWA para registrar partidos, torneos y campeones de FIFA. Single-file, sin build step.

## Características

- **3 formatos de torneo**: Liga (ida o ida/vuelta), Eliminatoria directa (con penales), Grupos + Copa (estilo Mundial, 2 o 4 grupos)
- **Sorteo automático** de fixture y llaves (algoritmo round robin + bracket con byes)
- **Tabla de posiciones** automática (Pts, DG, GF, orden FIFA)
- **Bracket visual** con avance automático de ganadores
- **Marcador tipo estadio** para registrar resultados
- **Palmarés** e historial de campeones
- **Export/Import JSON** para respaldo
- **PWA instalable** con funcionamiento offline

## Deploy en GitHub Pages

```bash
git init
git add .
git commit -m "FIFA Torneos v1.0"
git branch -M main
git remote add origin https://github.com/angulodev/FIFA-tracker.git
git push -u origin main
```

Luego en GitHub: **Settings → Pages → Source: Deploy from a branch → main / (root) → Save**

En unos minutos queda en: `https://angulodev.github.io/FIFA-tracker/`

## Stack

- React 18 (UMD) + Babel standalone — sin build
- CSS custom (tema "estadio nocturno" con acento volt)
- localStorage (`fifa_tracker_v1`)
- Service Worker (network-first)

## Datos

Todo se guarda localmente en el navegador. Usa **Equipos → Exportar datos** para respaldar antes de limpiar el navegador o cambiar de dispositivo.
