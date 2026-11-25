# Opgaver til IMPR Lektion 13

Det primære fokus i dagens opgaver er at arbejde med binære træer og kædede lister.

---

For de fleste af dagens opgaver vil det være passende at
1) implementere funktionen i et lille bibliotek, og
2) skrive en eller flere unit tests af funktionen

Specifikt til dagens opgaver kan du prøve at dele Kurts kode op i bibliotekskode og testkode. 
Du kan passende starte med dine tests, det er god brug af "top-down" programmering.

## Gruppeopgaver
Disse opgaver laves sammen i gruppen. Der er rigeligt med opgaver.
Arbejd grundigt med de opgaver, I kan nå, i den skemalagte tid.

### [Opgave A](src/opgave-a.c): Højde-funktion af binært træ
Dette er Kurt Nørmark's [opgave 12.7](https://homes.cs.aau.dk/~normark/impr-c/structures-flere-opgaver-slide-exercise-3.html).
Du kan tage udgangspunkt i programmet i filen [`opgave-a.c`](src/opgave-a.c).

> Højden af et binært træ defineres som højden af træets rod.
> 
> Højden af en knude K i træet er den længste sti fra K til et blad. 
> Med dette bliver højden af et blad altså 0.
> 
> Skriv en funktion i C der beregner højden af et træ. 
> Udgangspunktet (parameteren) skal være en pointer til en knude i træet. 
> Afprøv funktionen på forskellige træer.
> 
> I filen [`opgave-a.c`](src/opgave-a.c) er et godt udgangspunkt for denne opgave - dog givet i kontekst af binære søgetræer - 
> og svarende til [de programmer der er diskuteret i lektionsvideoen](https://laml.cs.aau.dk/cgi-bin/video2/get/show-video.cgi?video-id=video-linked-trees&course-id=impr&lecture-number=13&course-year=2026&video-width=840&lang=dk&video-start-time=24:34&auto-play=1).

---
### [Opgave B](src/opgave-b.c): Funktioner på cirkulære lister
Dette er Kurt Nørmark's [opgave 12.6](https://homes.cs.aau.dk/~normark/impr-c/structures-flere-opgaver-slide-exercise-2.html).
Du kan tage udgangspunkt i programmet i filen [`opgave-b.c`](src/opgave-b.c).

> I denne opgave skal du tage udgangspunkt i [diskussionen af cirkulære lister](https://laml.cs.aau.dk/cgi-bin/video2/get/show-video.cgi?video-id=video-linked-lists&course-id=impr&lecture-number=13&course-year=2026&video-width=840&lang=dk&video-start-time=24:25&auto-play=1) i videoen, som hører til denne lektion. 
> Jeg foreslår at du laver en cirkulær liste med punkter.
> 
> Start med at programmere en funktion der beregner listens længde: `length_of_circular_list`
> 
> Programmer dernæst de fire funktioner der hhv. indsætter og sletter det første og det sidste element i en liste:
> - `insert_head`
> - `insert_tail`
> - `delete_head`
> - `delete_tail`
> 
> Det forventes at alle pånær én af disse kan køres i konstant tid (altså uafhængig af listens længde). 
> Hvilken funktion er markant mindre effektiv end i de andre?
> 
> I filen [`opgave-b.c`](src/opgave-b.c) et udgangspunkt, som gør det lidt lettere at komme i gang:

---
### [Opgave C](src/opgave-c.c): En funktion der genkender et binært søgetræ
Dette er Kurt Nørmark's [opgave 12.8](https://homes.cs.aau.dk/~normark/impr-c/structures-flere-opgaver-slide-exercise-4.html).
Du kan tage udgangspunkt i programmet i filen [`opgave-c.c`](src/opgave-c.c).

> Programmer en funktion, `is_binary_search_tree`, der tager et binært træ som input, 
> og som returnerer hvorvidt dette træ er et (binært) søgetræ.
> 
> Afprøv funktionen på forskellige binære træer.
> 
> I filen [`opgave-c.c`](src/opgave-c.c) er der et godt udgangspunkt for denne opgave. 
> Det vil også være en god ide at konsultere denne del af [lektionsvideoen](https://laml.cs.aau.dk/cgi-bin/video2/get/show-video.cgi?video-id=video-linked-trees&course-id=impr&lecture-number=13&course-year=2026&video-width=840&lang=dk&video-start-time=19:36&auto-play=1), hvor et binært søgetræ defineres.
