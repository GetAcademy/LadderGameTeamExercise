I denne oppgaven skal vi se på stigespillet i enkel one player-versjon. Dere skal ikke nødvendigvis lage alt ferdig, og hvert team velger hvor langt dere vil gå. Jeg tenker: bruk maks. 2 timer på dette. Men bruk mer om dere finner det gøy og lærerikt.

![](https://fuzzbin.github.io/skolekoden/_images/stigespill_brett.png)

1. Lag en funksjon `createRow` som returnerer 9 div-er med et tall inne i hver rute. Funksjonen skal ta en parameter startValue som skal vises i den første ruten, samt en parameter til, change. Denne er enten +1 eller -1 og styrer om de følgende rutene får større eller mindre tall enn startruten. 

    _Forenklet versjon_: Lag to versjoner av `createRow`: `createRowPlus` og `createRowMinus` hvor den ene teller opp og den andre ned	

2. Bruk dette til å tegne opp hele brettet med riktige numre. Vi ser bort fra stigene og ulike farger foreløpig. 

3. Lag en funksjon `getLadderFrom`. Denne tar en parameter, `squareNo` - som representerer tallet i hver rute. Hvis det ikke starter noen stige i angitte `squareNo`, skal funksjonen returnere `null`. Ellers skal den returnere rutenummeret som stigen fører til. I denne funksjonen blir det bare en lang rekke av if-setninger. En for hver stige. 

4. Bruk `getLadderFrom` til å farge ruter med stige til høyere rutenummer grønne og ruter med stige til lavere rutenummer røde. Vi skal ikke markere rutene som stigene ender i - men dere kan legge til tekst, for eksempel “stige til 40” i ruten hvor stigen starter.

5. Frivillig: Lag en funksjon som sjekker om en stige ender i et bestemt `squareNo` - og bruk det til å fargelegge ruten hvor en stige ender enten lysegrønn eller rosa. 

6. Bruk MVC og en variabel `currentSquareNo`. Tegn opp en brikke i riktig rute - start på 1. For å teste dette, lag seks knapper som kaller `movePiece(1)`, `movePiece(2)` osv. opp til `movePiece(6)`. Sørg for at brikken flytter seg riktig antall steg når man trykker på disse knappene - og sørg for at brikken følger stigen om den kommer til en rute hvor en stige starter. 

7. Bytt ut de seks knappene med en knapp for å kaste en terning. Vis riktig terning på enkelt vis, for eksempel ved å bruke unicode: ⚀⚁⚂⚃⚄⚅

8. Kjenn igjen om brukeren har fullført spillet. Vis en melding hvis spillet er ferdig og tilby muligheten til å starte på nytt. 
