# Jugabilidad

**PROPUESTA — no canon.** Diseño desde cero para LFSim. Parte de [ESTRUCTURA](../historia/ESTRUCTURA.md), [REGLAS_PERSONAJES](../historia/REGLAS_PERSONAJES.md) y [PROGRESION](../historia/PROGRESION.md). Lo que aquí se llama «operación», «enfrentamiento» o «tablero» son nombres de trabajo.

## Objetivo

Que cada sesión tenga **cosas distintas que hacer** y que todas sean divertidas por sí mismas, sin dejar de contar la historia. El combate es lo más frecuente, pero no lo único: se alterna con exploración, deducción, contacto y decisiones.

## Pilares

1. **Ver para decidir.** El jugador ve lo que va a hacer cada amenaza antes de actuar. La dificultad está en elegir, no en adivinar.
2. **Elige, mira y tira.** Eliges una carta, ves la dificultad y la probabilidad, y entonces lanzas el d20. El azar nunca llega por sorpresa.
3. **Nunca hay suficiente.** Siempre falta una carta, un turno o una persona. Toda partida obliga a renunciar a algo.
4. **Combatir no es lo mismo que matar.** Contener, evacuar, proteger, observar o ahuyentar son tan importantes como golpear.
5. **Lo que pasa, se queda.** Heridas, muertes, pistas y frentes perdidos no se deshacen.
6. **Cada vida cambia las reglas.** El núcleo es el mismo, pero cada vida añade o quita una mecánica, para que ninguna se juegue igual.

## El ciclo de juego

```text
FRENTE ──elige una operación──▶ OPERACIÓN (mapa) ──▶ RESULTADO
  ▲                               │  enfrentamientos, peligros,                 │
  │                               │  hallazgos, civiles, contacto               │
  │                               ▼                                             ▼
  └──── el mundo avanza ◀── CAMPAMENTO (escuadra, una escena) ◀── TABLERO DE PISTAS
```

Una vuelta completa dura unos 15–25 minutos. Una vida tiene entre 4 y 6 vueltas, más los Moments de historia.

## Los seis modos

| Modo                   | Qué haces                                                                                   | Por qué divierte                                    | Referencias          |
| ---------------------- | ------------------------------------------------------------------------------------------- | --------------------------------------------------- | -------------------- |
| **Frente**             | Eliges una de dos o tres operaciones. Las que no eliges se resuelven sin ti.                | Elegir qué dejas caer; ver el mundo cambiar.        | XCOM, FTL            |
| **Operación**          | Avanzas por un mapa corto dentro del Umbral, eligiendo ruta mientras crece la inestabilidad. | Arriesgarte un nodo más por una pista o un rescate.  | Slay the Spire, FTL  |
| **Enfrentamiento**     | Combate por turnos: eliges cartas de acción que flotan sobre tu mano y lanzas un d20 por cada una. | Decidir con la probabilidad a la vista antes de cada tirada. | Into the Breach, Slay the Spire, Baldur's Gate 3 |
| **Tablero de pistas**  | Conectas pistas para formar hipótesis; una pista nueva puede tumbar una vieja.              | El «¡ajá!» de deducir tú, sin que te lo den hecho.   | Return of the Obra Dinn, Shadows of Doubt |
| **Contacto**           | Hablas con alguien del otro lado con una traducción incompleta que mejora poco a poco.      | Entender una lengua y decidir cuándo no disparar.   | Heaven's Vault, Chants of Sennaar |
| **Moments**            | Decisiones de historia: binarias, múltiples o con tiempo.                                   | Dilemas con coste; consecuencias que vuelven años después. | LifeSim, Reigns |

El **campamento** no es un modo de gestión: es una escena corta entre operaciones con la escuadra (una conversación, una herida que cuidar, una carta). Es el contraste que pide el canon ([C16](../lore/CANON_RULES.md)).

## Enfrentamiento (el combate)

El modo más frecuente: tiene que ser rápido, claro y con decisiones en cada acción.

**Cómo se ve**

- Arriba, las **amenazas**, cada una con su aguante, su defensa, su fuerza y su **intención** para esta ronda (atacar a alguien, cargar, ir a por los civiles, ensanchar la brecha, vigilar o huir).
- Abajo, una **mano abierta** de la que surgen **cartas flotando**, como si las estuviera invocando. Cada carta es una acción.
- La carta **Huir** está siempre en la mano. Elegir cualquier otra es decidir quedarse.

**Cómo se juega una acción**

1. Eliges una carta de la mano; sube y se coloca encima de la mano.
2. Si necesita objetivo, tocas la amenaza o al compañero.
3. La carta muestra la **dificultad y la probabilidad antes de tirar**: «Necesitas 12 o más · 45 %».
4. Puedes cambiar la dificultad con **Esforzarte** (−3, +1 estrés) o **Sobrecargar el Núcleo** (−6, crisis +1), y ver cómo cambia la probabilidad.
5. **Lanzas el d20.** El 20 natural es crítico (efecto mayor) y el 1 es pifia (falla y suma estrés).

Cada ronda robas una mano de **5 cartas + Huir** y puedes jugar **3**. Después actúan las amenazas cuya intención no hayas frenado. Puedes terminar la ronda antes si no quieres gastar más cartas.

**Cartas del mazo**

| Carta           | De quién | Dificultad          | Si sale bien                                                |
| --------------- | -------- | ------------------- | ----------------------------------------------------------- |
| Atacar          | Tú       | Defensa del objetivo | −2 aguante (−3 con crítico).                               |
| Proteger        | Tú       | Fuerza del objetivo | Anula su intención esta ronda.                              |
| Golpe de Núcleo | Tú       | Defensa + 3         | −3 aguante (−4 con crítico).                                |
| Observar        | Bram     | 10                  | Su defensa baja 5 hasta que lo golpeéis; un crítico da una pista. |
| Ahuyentar       | Bram     | Fuerza + 2          | Solo fauna: se va sin luchar.                               |
| Curar           | Ilse     | 9                   | −1 herida a un compañero.                                   |
| Evacuar         | Tú       | 8                   | 1 civil a salvo (2 con crítico). Solo en evacuaciones.      |
| Huir            | Tú       | 6 + 2 por amenaza   | Termina el combate como retirada. Si falla, os alcanzan.    |

**La escuadra es el mazo.** Si Ilse cae, sus cartas de curar dejan de aparecer. La confianza ganada en un descanso hace las cartas de ese compañero 2 puntos más fáciles.

**Consecuencias:** una intención que nadie frena hiere a alguien o se lleva civiles. Tú aguantas 3 heridas y tus compañeros 2. Si caes, la operación termina; en el juego completo puede ser el final de la vida.

**Resultado:** completado, parcial, fallido, retirada o abortado. Fallar no corta la historia: cambia el siguiente nodo y el informe del frente.

**Refuerzos anunciados:** algunas escenas avisan de que llegará otra amenaza en una ronda concreta, y el combate cambia a mitad.

**Fuera del combate, las mismas cartas.** Los peligros, rescates, hallazgos, descansos y contactos del mapa también se presentan como cartas sobre la mano. Las que tienen riesgo muestran su dificultad y se resuelven con el d20.

## Operación (el mapa)

- **Mapa corto** de 5–7 nodos con bifurcaciones, visible desde el principio.
- **Inestabilidad:** sube un punto en cada nodo. Al llegar al máximo hay que salir, y el último tramo es un enfrentamiento de extracción.
- **Nodos:** enfrentamiento, peligro (una decisión con tirada), hallazgo (una pista), civiles (un rescate con coste), descanso (curar o una escena con la escuadra) y contacto (raro).
- **Suministros** limitados: curar, reforzar o comprar un turno extra cuestan lo mismo.
- La gracia es apostar: el hallazgo está dos nodos más allá y la inestabilidad ya va por la mitad.

## Frente

- Cada periodo se ofrecen dos o tres operaciones en frentes distintos. **Solo se puede hacer una.**
- Las que no eliges se resuelven solas con lo que tenga el mundo. Lo verás en el siguiente informe: un frente que resistió sin ti, un refugio que cayó.
- Aquí se mueven los hilos del mundo de [ESTRUCTURA](../historia/ESTRUCTURA.md): figuras históricas, refugiados, conocimiento y contacto.

## Tablero de pistas

- Cada pista es una carta: de dónde viene, qué dice y cuánto se puede fiar uno.
- Conectas dos o tres pistas a una **hipótesis**. Si encajan, se refuerza; si una pista nueva la contradice, se marca y hay que revisarla.
- Tres hipótesis bien sostenidas forman una **síntesis**: la escalera de [PROGRESION](../historia/PROGRESION.md).
- El juego no te dice si tu hipótesis es la correcta hasta que una prueba la confirma o la tumba. Las pistas y su significado real están en el canon privado.

## Contacto

- Diálogo con alguien del otro lado. Lo que dice aparece con huecos; con cada contacto se llena un **glosario**.
- Eliges cómo interpretar cada frase. Una interpretación equivocada puede convertir un acuerdo en un enfrentamiento.
- Dentro de un enfrentamiento puede aparecer una amenaza que **no es una amenaza**: el jugador atento lo nota en su intención («proteger crías», «huir») y puede no disparar.

## Moments

Las decisiones de historia del canon ([MOMENTS](../lore/MOMENTS.md)): binarias, múltiples, cronometradas, mantener o arriesgar, priorizar. Aparecen entre modos y dentro de ellos (por ejemplo, una orden que desobedecer a mitad de una operación).

## Progresión sin estadísticas que suben

- **No hay experiencia ni niveles.** Lo que cambia es lo que tienes y lo que te ha pasado.
- **Escuadra:** cada compañero aporta sus cartas al mazo. La confianza las hace más fáciles; si muere, desaparecen.
- **Equipo:** pocos objetos con un efecto claro, ganados en operaciones. No hay tienda.
- **Heridas y cicatrices:** cierran acciones o papeles y abren escenas.
- **Núcleo** (Despertados): la carta de Golpe de Núcleo y la sobrecarga. El rango cambia cuánto baja la dificultad la sobrecarga y cuántas cartas de Núcleo hay en el mazo, nunca la regla del juego.

## Cada vida cambia las reglas

| Vida | Lo que añade o quita                                                                                           |
| ---- | -------------------------------------------------------------------------------------------------------------- |
| 1    | **Sin Núcleo y con poca fuerza.** Golpear apenas sirve; se gana evacuando y protegiendo. Mecánica propia: el **pánico** de los civiles, que se calman o se dispersan. |
| 2    | **Observación como arma.** Los instrumentos añaden cartas de lectura; el tablero de pistas tiene más peso. Mecánica propia: **muestras** que hay que sacar intactas. |
| 3    | **Núcleo y sobrecarga.** Las escenas más duras y las brechas más grandes. Mecánica propia: **crisis del Núcleo** si se abusa de la sobrecarga. |
| 4    | **Contacto.** Intenciones ambiguas y la opción de no disparar. Mecánica propia: el **glosario** y los acuerdos que se rompen. |
| 5    | **Mando.** Se dirigen varios equipos a la vez en una campaña. Mecánica propia: **asignar escuadras** a frentes, como un enfrentamiento a gran escala. |

## Prototipo

[`prototipos/operacion.html`](../prototipos/operacion.html) es un prototipo gris del ciclo **frente → operación → enfrentamientos → resultado**, con el tipo de reglas de la vida 3. Sirve para comprobar si el enfrentamiento divierte antes de construir lo demás. Se abre directamente en el navegador, sin servidor; `?semilla=N` repite una partida. El tablero de pistas, el contacto completo y el campamento aún no están prototipados.

Con un jugador automático sencillo y 40 partidas por operación, «Bombeo» se completa un 57 %, queda parcial un 27 % y el protagonista cae un 15 %; «Grúas», 45 %, 45 % y 10 %. Son cifras orientativas y no sustituyen a probarlo jugando. En móvil, los nombres largos de las cartas se recortan cuando la mano está llena.

## Preguntas abiertas

- Plataforma principal (móvil, PC o ambas). Afecta al tamaño del mapa y a cómo se abre el abanico de cartas.
- Motor definitivo. El prototipo es HTML sin dependencias para probar reglas, no una decisión técnica.
- Cuánto debe durar una vida en minutos de juego.
