# AyudantiaPOO

Enzo Loren

La clase Carta representa una carta del naipe inglés, con dos atributos: valor y pinta. El valor puede ser un número del 1 al 10, o una letra que representa a la Jota, la Quina, el Kaiser o el As. La pinta puede ser Corazón, Trébol, Diamante o Pica. La clase Carta tiene un método llamado getValor(), que devuelve el valor numérico de la carta según las reglas del juego (10 para las letras y 11 para el As).

La clase Baraja representa un conjunto de 52 cartas, con un atributo llamado cartas, que es una lista que almacena objetos de la clase Carta. La clase Baraja tiene dos métodos: mezclar(), que ordena aleatoriamente las cartas de la lista, y repartir(), que devuelve la primera carta de la lista y la elimina de la misma.

La clase Jugador representa a una persona que participa en el juego “Blackjack”, con dos atributos: nombre y mano. El nombre es una cadena de caracteres que identifica al jugador, y la mano es una lista que almacena objetos de la clase Carta. La clase Jugador tiene tres métodos: pedirCarta(), que recibe un objeto de la clase Baraja como parámetro y añade a su mano la carta que devuelve el método repartir() de la baraja; plantarse(), que indica que el jugador no quiere recibir más cartas; y calcularPuntaje(), que suma los valores numéricos de las cartas de su mano y devuelve el resultado.

La clase Crupier representa al encargado de dirigir el juego “Blackjack”, con dos atributos: nombre y mano. El nombre es una cadena de caracteres que identifica al crupier, y la mano es una lista que almacena objetos de la clase Carta. La clase Crupier hereda los métodos pedirCarta(), plantarse() y calcularPuntaje() de la clase Jugador, y además tiene un método propio llamado mostrarCarta(), que devuelve la primera carta de su mano sin eliminarla de la lista.

La clase Juego representa al juego “Blackjack” en sí mismo, con tres atributos: baraja, crupier y jugadores. La baraja es un objeto de la clase Baraja, el crupier es un objeto de la clase Crupier, y los jugadores es una lista que almacena objetos de la clase Jugador. La clase Juego tiene cuatro métodos: iniciar(), que crea e inicializa los atributos de la clase; repartirInicial(), que reparte dos cartas a cada jugador y al crupier usando el método pedirCarta() de cada uno; jugar(), que permite a cada jugador decidir si quiere pedir más cartas o plantarse usando los métodos pedirCarta() y plantarse() respectivamente; y determinarGanador(), que compara los puntajes de cada jugador y del crupier usando el método calcularPuntaje() de cada uno, y devuelve el nombre del ganador o un mensaje indicando si hay empate o si todos han perdido.


Elegí las clases Carta, Baraja, Jugador, Crupier y Juego porque me parecieron las más adecuadas para representar los elementos involucrados en el juego Blackjack. Cada clase tiene sus propios atributos y métodos que definen sus características y comportamientos.
Elegí las relaciones de asociación, agregación y herencia porque me parecieron las más apropiadas para representar las conexiones entre las clases. La asociación indica que una clase usa o conoce a otra clase, en este caso la clase Juego usa objetos de las clases Baraja, Crupier y Jugador. La agregación indica que una clase contiene o está compuesta por otra clase, en este caso la clase Baraja contiene objetos de la clase Carta.
