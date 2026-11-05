# HIGHFLY FURY — SKILL LAB L25

Laboratorio **independiente** para probar 15 habilidades, VFX propios y Ruptura Aérea sin modificar la aplicación HIGHFLY principal.

### Jugar en Android horizontal o PC

**https://drakenhok-star.github.io/HIGHFLY-FURY-SKILL-LAB/**

La publicación utiliza una única escena con **tres esqueletos quietos y un dragón Quaternius volador animado**. Los cuatro objetivos reciben daño real; no perseguirán al jugador ni entregarán XP o loot.

### Control L25

- **15 skills** en cinco kits: Guinevere, Dyrroth, Tigreal, ClaudeCraft Mago y ClaudeCraft Pícaro. S1/S2/S3 usan los botones existentes, sin duplicar el HUD.
- **ENFOCAR**: botón compacto junto al ATK; selecciona **solo monstruos voladores**. Los terrestres conservan AIM manual.
- Con un volador enfocado, **ATK dispara proyectiles energéticos** de corta cadencia. **4 impactos confirmados en 4,5 s** rompen la estabilidad del dragón.
- **Ruptura Aérea**: el dragón desciende progresivamente, permanece vulnerable a combate terrestre varios segundos y luego recupera el vuelo. **ATK 1-2-3-4 de FURY P16 sigue intacto** cuando el enemigo no está volando enfocado.
- **CANCELAR SKILL** aparece al apuntar junto a **MOCHILA**; cancelar no consume MP/Energía ni cooldown.
- Joystick, movilidad FURY P16, cámara híbrida, salto/dash, cuarto ATK direccional, inventario y mapa originales preservados.

### Publicación, pruebas y recuperación

- Código original y versión para regresiones: [HIGHFLY-ORIGIN-DEMO — L25](https://github.com/drakenhok-star/HIGHFLY-ORIGIN-DEMO/tree/l25-vfx-ruptura-aerea-20261105).
- [Auditoría de VFX, referencias MIT/CC0 y restricciones](https://github.com/drakenhok-star/HIGHFLY-ORIGIN-DEMO/blob/l25-vfx-ruptura-aerea-20261105/docs/L25_VFX_DEPENDENCY_AUDIT_AND_AERIAL_RUPTURE.md).
- [CI L25 aprobada](https://github.com/drakenhok-star/HIGHFLY-ORIGIN-DEMO/actions/runs/42114983742).
- **Versión L24 de recuperación**: rama original `l24-unified-island-dragon-and-bots-20261105` y backup de este repositorio `backup-pages-l24-unified-island-20261105`.
- GitHub Pages se publica desde un **commit SHA fijo** del repo de origen mediante `.github/workflows/pages.yml`, sin clonar un segundo laboratorio ni transferir cambios a la app principal.

**Licencias:** código MIT y recursos CC0 con procedencia individual trazable. Ningún PNG/atlas/GLB/SFX ClaudeCraft que no haya aprobado la whitelist legal se importa al laboratorio. Recursos «With the project only», CraftPix y paquetes Unity no portables quedan fuera.

**Alcance de la validación:** CI verifica sintaxis, arquitectura y lógica; no sustituye la comprobación visual ni la medición real de rendimiento en Samsung S23 Ultra horizontal. Los 15 perfiles VFX son la nueva base técnica premium; el acabado visual final debe evaluarse en el dispositivo.
