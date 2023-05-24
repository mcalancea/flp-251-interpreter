# flp-251-interpreter

Salut! Acesta este un interpretor compus din soluțiile laboratoarelor 1-6. Îl puteți folosi ca punct de pornire pentru testul de laborator din 25 mai (12:00 - 14:00, Lab 303).

Testul va conține mai multe exerciții independente, fiecare cerându-vă să implementați o funcționalitate (minoră) peste cele deja existente. 

## Exemplu (Multi-argument lambdas)

O convenție comună în scrierea lambda-expresiilor (pe care ați întâlnit-o poate și la curs) spune că se pot introduce mai multe variabile legate în fața unui singur simbol lambda. Spre exemplu, este mai succint să scriem `\x y z -> x (y z)` decât `\x -> \y -> \z -> x (y z)`. În momentul de față interpretorul acceptă doar a doua varianta. Să numim prima variantă forma "multi-arg".

### a).
Modificați interpretorul astfel încât să acceptați notația multi-arg pentru lambda-expresii (i.e, REPL-ul să trateze aceste expresii în mod echivalent cu forma lor explicită acceptată).

### b).
Modificați interpretorul astfel încât afișați orice lambda-expresie în forma multi-arg. Spre exemplu, dacă se introduce în REPL expresia `\x -> \y -> x y t`, ar trebui să o afișați ca `\x y -> x y t`.
Cu alte cuvinte, comprimați lambda-abstracțiile sub un singur simbol lambda oricând este posibil.

Detaliile implementării nu contează, atât timp cât obțineți comportamentul dorit. 

Pentru a crea un branch nou puteți folosi comanda:

```
git checkout -b multi-arg`
```

Când terminați exercițiul, nu uitați să adăugați schimbările într-un commit:

```
git add -u
git commit -m "Add multi-arg functionality."
```

În final, reveniți pe branch-ul main și creați un ZIP din branch-ul `multi-arg`:

```
git checkout main
git archive --output=./multi_arg.zip --format=zip multi-arg
```
