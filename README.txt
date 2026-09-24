LA SUSTANCIA — GYM PET v2

Rediseño de mascotas + reparación de animaciones.

Estructura:
- index.html: aplicación web responsive.
- assets/pets/: sprites pixel retro separados (90 PNG: 3 mascotas × 3 niveles × 10 estados).

Diseño de mascotas:
- Las tres mascotas comparten la misma familia visual hasta la etapa final.
- Ojos siempre "00".
- Nivel 1: cabeza grande + elementos tipo oreja y manos flotantes.
- Nivel 2: mismo diseño base con cuerpo/actitud más desarrollados.
- Nivel 3: diferencia física entre Macho y Hembra; Robot mantiene diseño neutro.
- Robot: paneles laterales de cabeza inspirados en mechas anime; en Retro la silueta es completamente cuadrada.
- Macho/Hembra: esquinas suavemente curvas; los detalles de orejas/accesorios pueden variar ligeramente.
- Retro usa spritesheets de 6 frames con fondo transparente e interpolación pixel-crisp.

Animaciones:
- Idle Retro ahora se reproduce continuamente, no solo durante una acción.
- Todas las acciones Retro usan sus 6 frames en loop mientras están activas.
- Al terminar una acción se vuelve a Idle automáticamente.
- La animación moderna también tiene idle continuo y movimientos de acción más notorios.
- Se mantiene el sistema de acciones existente: interacción, pesas, running, yoga, combate, varios, descanso, creatina y level-up.
- Los sprites Retro ya no dependen de un elemento que aparezca invisible por falta de fondo/transparencia.

Características principales:
- Modos Claro, Oscuro y Retro.
- En Retro, solo la mascota usa pixel art; la interfaz mantiene su estructura moderna y la paleta LCD.
- Macho, Hembra y Robot, con evolución visual por nivel.
- 4 rutinas iniciales, pero cantidad ilimitada.
- Edición/reordenamiento de rutinas y ejercicios.
- Una recompensa de entrenamiento por día: XP + Estamina al 100%.
- 00 (Creatina): máximo 1 uso diario y +30% de Estamina.
- Historial de peso por ejercicio y calendario de consistencia.
- Persistencia mediante localStorage.
- Migración automática desde la versión anterior laSustanciaGymPet_v1 cuando existe.

Para probar localmente:
1. Mantén index.html junto a la carpeta assets.
2. Abre index.html en un navegador moderno o publícalo en cualquier hosting estático.
3. Para el flujo QR, apunta el QR a la URL pública de index.html.
