# Macarroners Spot — Cartoon + Arcade

## Qué incluye
- Rediseño completo con estética cartoon: contornos gruesos, sombras tipo cómic, colores vivos, tarjetas inclinadas y animaciones.
- Nueva jerarquía: portada → zona arcade → grupo → biblioteca de fotos → museo del meme → ubicación.
- **Meme Battle** multijugador: sala con código, rondas configurables, plantillas, tiempo de creación, envío de memes, votación y clasificación.
- **Insight Spot** multijugador: turnos por protagonista, pregunta abierta, respuestas de los demás, elección de respuesta favorita y puntuación.
- Se conserva el HTML anterior como `original-index-referencia.html` para consultar funciones previas (Impostor y Paper Spot).

## Ejecutar
1. Descomprime la carpeta.
2. Abre `index.html` en un navegador moderno. Para publicar, súbelo a GitHub Pages o cualquier hosting HTTPS.
3. Para partidas entre móviles, todos necesitan internet. El anfitrión debe mantener abierta la página durante la partida.

## Imágenes
Copia tus archivos dentro de `imagenes/`:
- `banco.jpg`
- `aran.jpg`, `javi.jpg`, `manel.jpg`, `laia.jpg`, `paula.jpg`, `marta.jpg`, `marcos.jpg`, `adri.jpg`, `rafa.jpg`, `cristian.jpg`
- `foto1.jpg` a `foto6.jpg`
- `meme1.jpg`, `meme2.jpg`, `meme3.jpg`

Si una foto no existe, se muestra un marcador de posición.

## Multijugador y límites
Los dos juegos nuevos usan PeerJS 1.5.5 desde CDN para señalización y WebRTC DataChannels para comunicar los móviles. No se necesita servidor propio, pero sí conexión a internet y que el anfitrión permanezca conectado. El estado de la partida lo mantiene el anfitrión; si cierra la pestaña, la sala se pierde. El proyecto no incluye cuentas, persistencia de partidas ni un backend dedicado.

## Nota
La versión anterior se conserva como referencia, pero sus juegos antiguos no se han integrado dentro del nuevo menú. Puedes consultarla en `original-index-referencia.html`.


## Juegos incluidos en esta versión

La edición integrada incluye cuatro juegos: **Meme Battle**, **Insight Spot**, **Impostor** y **Paper Spot**. Los dos últimos se han recuperado e integrado en la misma zona arcade y comparten el diseño cartoon. Las salas multijugador usan PeerJS/WebRTC: el anfitrión debe mantener la pestaña abierta y todos los jugadores necesitan conexión a Internet.

Para jugar desde móviles, publica la carpeta completa en un hosting HTTPS (por ejemplo GitHub Pages). No abras el HTML mediante `file://`, ya que las conexiones entre navegadores necesitan un origen web.
