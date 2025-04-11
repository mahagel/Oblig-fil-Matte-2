# Oblig-fil-Matte-2
Nevralt nettverk helt fra bunn (C++)

zip filen skal inneholde alt du trenger, for å kjøre i VScode (Tror jeg)

Dette er en veldig enkel modell av et nevralt nettverk, som tar inn et vilkårlig antall inputverdier, og gir ut et vilkårlig antall outputverdier. 
Etter trening, skal nettverket ha lært hva som er forventet output fra en gitt input av seg selv, og deretter visualisere resultatet.
Nettverket følger grunnleggende prinsipper for maskinlæring og er veldig dårlig optimalisert, men det fungerer og det var målet for prosjektet.
Dvs: Nettverks-struktur med input-lag, skjulte lag og output-lag med nevroner som aktiveres med hensyn på bias, vekter og de forrige aktiveringene.
Parametrene blir tilfeldig initialisert, og informasjonen fra input-laget flyter deretter gjennom nettverket i det man kaller forward pass og man ender opp med en tilfeldig output.
Deretter sammenlikner man output og forventet output for input-laget, og får en tapsfunksjon, gitt av parametrene.
For læringen ønsker man å finne bunnpunktet til tapsfunksjonen, og gjør dette ved å gange vektene og biasene med en skalert verdi av de negative gradientene til tapsfunksjonen. Dette kalles backwards pass eller backpropagation.
Etter å ha gjort dette MANGE ganger for forskjellige input og tilhørende output, ender nettverket opp i et lokalt minima av tapsfunksjonen, som betyr at forventet output går mot den faktiske outputen.

I tillegg visualiserer jeg treningen ved at man kan se hvordan nevronene aktiveres (nevronene blir større for høyere aktivering) og at vektene (linjene mellom nevronene) blir større eller mindre.

Underveis i prosjektet har jeg brukt copilot mye for debugging av programmet i tillegg til informasjon og ideer om hvordan jeg kan løse visse problemer.
Jeg har også brukt ChatGPT og Deepseak for problemløsning, generering av test-funksjoner og debugging.

For inspirasjon og informasjon om hvordan nevrale nettverk fungerer har jeg hovedsakelig brukt threeBlueoneBrown sin serie om nevrale nettverk og Artem Kirsanov sin video om backpropagation.
Imidlertid har jeg sett mange andre videoer jeg ikke husker navnet på, som også har hjulpet med grunnleggende forståelse og inspirasjon.
