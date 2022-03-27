## stati_cast

Beim Wort `cast` handelt es sich im technische und wörtlichen Sinne um das Verb `gießen`. Es beschreibt anschaulich, dass ein Eingangsobjekt in eine _neue Form_ `gegossen` wird.

Der `static cast` wird benutzt, um eine `implizite` Konvertierung umzudrehen. Es wird also vom Programmierenden erwartet, dass genau gewusst wird, welcher Typ das Objekt hat oder haben kann. Die Konvertierung vollführt dann **keine** Überprüfungen zur Laufzeit.

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

