# HIGHFLY Skill Lab L21 — motor FURY P16

Laboratorio público y aislado de skills, combos, apuntado y VFX para HIGHFLY.

**Motor y código principal:** [HIGHFLY-ORIGIN-DEMO](https://github.com/drakenhok-star/HIGHFLY-ORIGIN-DEMO), rama interna `p21-fury-skills-full-training-pages-20261105` (versión pública **L21**). El motor FURY P16 tiene prioridad: joystick 360°, combo 1–2–3–4 con daño confirmado, remate direccional desde ATK, movimiento, dash y salto. Skills y VFX son adaptadores.

Este repositorio NO contiene una segunda copia permanente del motor, ni modifica el Pages original. El workflow de GitHub Actions descarga la rama de laboratorio aprobada y la sirve desde este repositorio independiente.

## Probar

Cuando el workflow de Pages haya superado pruebas y se habilite **Settings → Pages → Build and deployment → GitHub Actions**, la dirección será:

https://drakenhok-star.github.io/HIGHFLY-FURY-SKILL-LAB/

**Pruebas:** tres esqueletos quietos de forma predeterminada (o uno, opcionalmente); reciben daño real, lanzamiento direccional, stuns y efectos sin perseguir al jugador ni otorgar XP. Cámara híbrida predeterminada.

## Cómo publicar una versión verificada

1. Verificar que los tests de la rama L21 estén en verde en el repo de origen.
2. Entrar en **Actions → Publish isolated HIGHFLY Skill Lab → Run workflow** en ESTE repositorio; indicar el commit aprobado de P20 para desplegar exactamente ese código.
3. La publicación es independiente; nunca sobreescribe el sitio de HIGHFLY-ORIGIN-DEMO.

Los recursos privados KayKit Complete SOURCE y los assets de terceros sin licencia compatible quedan excluidos.

## Migración futura

Al aprobar las skills, los cambios viajan hacia la demo principal mediante PR selectivo: `src/skillslab/**`, adaptadores VFX/aim y solo pequeños hooks de integración probados. No sustituir `src/player/player.js` ni `src/combat/combat.js` enteros. Verificar licencias, input táctil y performance en S23 Ultra antes del merge.

**Convención:** **P** significa versión de la aplicación Principal; **L** significa versión del Laboratorio. Los nombres técnicos existentes de las ramas o módulos no se modifican.
