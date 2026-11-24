# Nowy Etap i Divory: prototypy stron

Statyczne prototypy, bez kroku budowania.

- `index.html`: strona główna repozytorium. Prototyp Nowy Etap: strona startowa, quiz i Plan Rozwodu.
  Plik jest generowany. Nie edytuj go ręcznie.
- `nowy-etap/index.html`: źródło prototypu Nowy Etap. Tu wprowadza się zmiany.
- `nowy-etap/build.py`: opakowuje źródło w pełny dokument i zapisuje `index.html` w katalogu głównym.
- `nowy-etap/img/`: logo.
- `divory/`: strona produktu Divory ze zdjęciami.

## Po każdej zmianie prototypu

```bash
python3 nowy-etap/build.py
```

## Wersje lejka w prototypie

Przełącza się je w menu „Prototyp” na stronie startowej albo parametrem w adresie (`?v=a`, `?v=b`, `?v=c`).

- **A**: plan od razu, rezerwacja rozmowy na stronie planu, kod SMS.
- **B**: e-mail, termin, numer do rozmowy telefonicznej, potem plan.
- **C** (domyślna): e-mail, termin spotkania online, numer na SMS z przypomnieniem, potem plan.

Strona ma znacznik `noindex`, bo zawiera dane demo.
