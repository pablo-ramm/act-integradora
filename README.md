# act-integradora
## Situacion a simular
En esta actividad se buscó simular el comportamiento del covid-19 en la sociedad, simulando contagios entre personas y cuantas de estas personas mueren  por este virus.

### Agentes
En esta actividad el modelo solo cuenta con un tipo de agente, una persona, la cual puede tener 3 estados: no contagiado, contagiado y muerto. Cada celda en el tablero representa a un agente persona y su estado dependera a su vez del estado de sus vecinos.

### Interaccion entre agentes
La simulación iniciaba con 10,000 agentes sobre el tablero de los cuales el 33% iniciaba con un estado portador del virus mientras que el resto en un estado no contagiado aún. Para que un agente no contagiado cambie su estado a contagiado este tiene que percibir 4 o más agentes a su alrededot con este estado para que el suyo tambien cambie. Una vez portador del virus, este agente tiene un 10% de probabilidad de cambiar su estado a muerto, este estado no afecta de alguna forma a los agentes que lo rodean.

### Entorno
El entorno de estos agente consta de 8 vecinos agentes todos de tipo persona, los pecibiran y dependiendo del estado de estos el suyo podrá cambiar, el muerto o no contagiado no tienen una repercusión directa en el estado del agente.

### Variables y parametros
Algunos parametros que modelan el funcionamiento es el numero de agentes colindantes con estado de infectado que un agente no infectado tiene que tener para cambiar su estado, en esta caso se requiere de 4 agentes aledaños. Otra variable es la posbilidad de muerte de un agente recien infectado el cual es del 10%.

### Simulación
La simulacion inicia en una sotuacion inicial con un tercio de los agentes totales contagiados, a traves de pasos cada agente podrá cambiar su estado dependiendo su entorno, todo los estados de los agentes son calculados en base al estado que tenia el tablero en el momento antes del paso, no tomando en cuenta el estado futuro que tendrian los agentes con este acomodo en el tablero, por lo que en el siguiente paso todo los agentes que se les calculo un estado diferente hacen el cambio al mismo tiempo para el calculo en la siguiente iteración.

### Resultados
Al final de una simulacion con 100 iteraciones todo el tablero se llena con agentes de solo 2 estados, muertos o contagiados, en su gran mayoria contagiados ya que la probabilidad de muerte era muy pequeña, para tener resultadoos diferentes se podria intentar iniciar con un porcentaje menor de contagiados o cambiar las variables.

### Link Repo

