# HIGHFLY FURY — SKILL LAB L26

Laboratorio **único e independiente** de 15 habilidades, VFX recuperados y combate aéreo. Un mapa con tres esqueletos quietos y un dragón Quaternius animado. No sustituye la app principal.

## Probar en móvil horizontal o PC

https://drakenhok-star.github.io/HIGHFLY-FURY-SKILL-LAB/

**Controles L26:**
- ENFOCAR solo voladores. Con dragón enfocado, ATK dispara energía; cuatro impactos reales provocan Ruptura Aérea y permiten continuar con el combo terrestre.
- EDITAR HUD → seleccionar «ENFOCAR VOLADOR» o arrastrar el botón → cambiar TAMAÑO, OPACIDAD y POSICIÓN → GUARDAR. Si ya había una disposición personalizada, NO reubicar a la fuerza ATK/USAR.
- Layout nuevo: ATK arriba, USAR abajo a su izquierda y ENFOCAR abajo a su derecha.
- CANCELAR SKILL sigue al control MOCHILA y no consume recursos/cooldown.
- Cinco kits con 15 habilidades: Guinevere, Dyrroth, Tigreal, ClaudeCraft Mago y ClaudeCraft Pícaro.

## Recuperación visual

Las seis habilidades basadas en World of ClaudeCraft 0.44.7 tienen efectos específicos de recreación MIT:
- Fireball: núcleo 3D, preparación e impacto incendiario confirmado.
- Meteorito: telegraph, columna descendente, tierra fragmentada y detonación a tiempo.
- Frost Nova: anillo de escarcha y pilares instanciados emergentes con cristales sobre víctimas.
- Backstab: estocada discreta de sombra solo si alcanza un enemigo.
- Kidney Shot: ataduras, golpe vertical y estrellas de aturdimiento al impacto.
- Charge: estela física, desplazamiento y fractura de choque cuando termina el dash.

Las nueve habilidades de estilos MOBA son recreaciones propias HIGHFLY con efectos originales. No utilizamos arte, sprites, atlas, audio o animaciones comerciales de otros juegos.

**Importante:** los efectos legales usan los parámetros/gramática del código MIT original, pero no son reproducciones pixel-perfect de medios visuales restringidos. La calidad final debe comprobarse en teléfono real.

## Repositorio y exportación

- [Implementación L26 aislada](https://github.com/drakenhok-star/HIGHFLY-ORIGIN-DEMO/tree/l26-hud-editor-vfx-recovery-20261105).
- [Informe de recuperación VFX y guía de exportación](https://github.com/drakenhok-star/HIGHFLY-ORIGIN-DEMO/blob/l26-hud-editor-vfx-recovery-20261105/docs/L26_VFX_RESTORATION_HUD_AND_EXPORT.md).
- [Catálogo puro de 15 skills para la demo](https://github.com/drakenhok-star/HIGHFLY-ORIGIN-DEMO/blob/l26-hud-editor-vfx-recovery-20261105/src/skillslab/skill-catalog-export-l26.js).
- Prueba automatizada Chrome móvil 915×412, con captura en GitHub Actions. No es benchmark de GPU Samsung.

### Recuperación y protección

- La versión anterior L25 está conservada en la rama original y en este repositorio bajo backup-pages-l25-ruptura-aerea-20261105.
- El Pages independiente despliega un commit SHA concreto aprobado de la rama laboratorio en HIGHFLY-ORIGIN-DEMO, no la rama principal.
- Nunca se publica aquí KayKit SOURCE adquirido ni archivos de terceros no acreditados.
- **FURY P16 no ha sido reemplazado**, tampoco jugador, mundo, cámara, joystick, cuarto ATK ni otras mecánicas del motor.
- Migrar a la demo principal **solo mediante adapter selectivo y QA**, sin copiar boot.js ni los cuatro objetivos de entrenamiento.

Convención HIGHFLY: **L** laboratorio de habilidades; **P** app principal.
