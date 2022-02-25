## stati_cast

Ich glaube das es bei dem `cast` um das Verb `gießen` handeln soll. Es beschreibt anschaulich, dass ein Eingangsobjekt in eine _neue Form_ `gegossen` wird.

Es  benutzt um eine `implizite` Konvertierung umzudrehen. Es wird also vom Programmierer angenommen, dass es genau den neuen Typ hat. Die Konvertierung vollführt dann **keine** Überprüfungen zur Laufzeit.

> im·pli·zit
> 1. mit enthalten, mit gemeint, aber nicht ausdrücklich gesagt "implizite Drohungen Forderungen"
> 2. nicht aus sich selbst zu verstehen, sondern logisch zu erschließen "Partizipialkonstruktionen sind implizit"

Es wird einfach verwendet, wenn bekannt ist, welches Objekt zu erwarten ist:

```c++
void meineFunktion(void* eingangsVoidZeiger)
{
  MeineKlasse* vonVoidZeiger = static_cast<MeineKlasse>(eingangsVoidZeiger);
  ...
}

int main() {
  MeineKlasse meineKlasse;
  meineFunktion(&meineKlasse); // Hier wird die Referenz auf meien Klasse übergeben
}
```

## dynamic_cast

Der dynamische

## reinterpret_cast

## const_cast

