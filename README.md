# Clase-5-Cultura-Digital
Clase 5 Cultura Digital 11-5-2026

Este codigo es un juego sencillo (Juego del dinosaurio en C++)


Simula el famoso juego del dinosaurio de Chrome en la consola usando caracteres ASCII. El jugador controla un dinosaurio que corre y debe saltar sobre cactus que aparecen desde la derecha. El juego se vuelve más rápido con el tiempo y guarda el récord de la sesión.
El programa tiene un tablero de texto de 60 columnas por 8 filas. El dinosaurio siempre está en la misma columna y los cactus se mueven de derecha a izquierda para simular el movimiento, buscando tocar al dinosaurio para que el jugador pierda.
El salto funciona con una variable de velocidad que empieza negativa (el dino sube) y aumenta cada frame por la gravedad hasta que el dino vuelve al suelo. Los cactus son estructuras simples con una posición y un estado activo o inactivo; cuando salen del tablero se reutilizan.
El juego detecta colisiones comparando si un cactus ocupa la misma columna que el dinosaurio mientras este está en el suelo. Si coinciden, el juego termina. Cada 50 puntos el juego reduce el tiempo de espera entre frames, haciendo todo más rápido.
Todo esto se repite en un bucle que sigue el mismo orden cada frame: leer tecla, mover objetos, detectar colisión, dibujar y esperar.
