# Debugging

Jeg brugte IntelliJ IDEA's **debugger tool** til at undersøge og rette de tre fejl i projektet. Ved fejlen med de kun horizontale battleships satte jeg et **breakpoint** ud for metoden, der laver spillepladen, for at stoppe op ved denne metode og dykke ned i de enkelte trin herefter. Jeg brugte **step over** og **step into** til at følge programmets flow. Jeg brugte også vinduet med variable til at undersøge værdier og udtryk undervejs. Dertil brugte jeg **evaluate** til at undersøge om udtryk ændrede sig som forventet ved hver kørsel.

Ved fejlen med den mangle "Ship sunk!"-besked, satte jeg et **breakpoint** ud for metoden, der generer trækkene i spillet. Igen brugte jeg **step over** og **step into** til at følge programmets flow, indtil jeg fandt det udtryk, der håndterer hits. Her brugte jeg **conditional breakpoints** i koden for at undersøge hvad der sker, når skibet er ramt tre gange.

Ved fejlen med ArrayIndexOutOfBoundsException brugte jeg et **exception breakpoint** til at få debuggeren til at stoppe præcis, da den exception opstod. I min version af IntelliJ foreslog den selv at jeg tilføj et exception breakpoint og derfor var det endnu hurtigere klaret, end i videoen. Knappen udfører stadig den samme handling for mig. Derefter kørte jeg programmet indtil den fandt det indeks, der lå uden for arrayets grænser.

Efter at have rettet fejlene kørte jeg programmet igen med og uden debug mode for at kontrollere, at rettelserne virkede.

**Step over** brugte jeg ikke ret meget, men jeg anerkender, at den kan bruges til at gå et skridt tilbage fra et kald, hvilket vil være nyttigt ifm. debugging af større programmer.
