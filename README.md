<div align="center">

# Digital Universe

**Zobacz, co AI wie o Tobie.** Dashboard z mapą powiązań, osią czasu i projektami, zbudowany z danych od ChatGPT, Claude, Gemini i innych.
<br>*See what AI knows about you. A dashboard with a connections map, timeline and projects, built from data provided by ChatGPT, Claude, Gemini and others.*

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
![Single file](https://img.shields.io/badge/single%20file-HTML-blue)
![Offline](https://img.shields.io/badge/works-offline-brightgreen)
![No dependencies](https://img.shields.io/badge/dependencies-none-lightgrey)

**MrPrompt – Centrum Otwartych Innowacji**

**[Polski](#-polski) | [English](#-english)**

</div>

---

## 🇵🇱 Polski

### Spis treści
- [O projekcie](#o-projekcie)
- [Funkcje](#funkcje)
- [Stack technologiczny](#stack-technologiczny)
- [Wymagania](#wymagania)
- [Instalacja](#instalacja)
- [Uruchomienie](#uruchomienie)
- [Użycie](#użycie)
- [Pokój wspomnień (bez aplikacji)](#pokój-wspomnień-bez-aplikacji)
- [Format danych](#format-danych)
- [Prywatność](#prywatność)
- [Struktura projektu](#struktura-projektu)
- [Testy](#testy)
- [Współtworzenie](#współtworzenie)
- [Licencja](#licencja)
- [Kontakt](#kontakt)

### O projekcie
Asystenci AI (ChatGPT, Claude, Gemini i inni) zapamiętują szczegóły z Twoich rozmów. Po wielu rozmowach trudno wiedzieć, co dokładnie o Tobie wiedzą.

**Digital Universe** to jedna aplikacja w jednym pliku HTML, która pomaga to zobaczyć:

1. kopiujesz z aplikacji gotowe polecenie i wklejasz je do swojego AI,
2. AI odpowiada ustrukturyzowanymi danymi (JSON) z tym, co o Tobie wie,
3. wklejasz odpowiedź do aplikacji, a ona buduje czytelny dashboard: mapę powiązań, oś czasu, projekty, umiejętności, wartości i cele.

Aplikacja jest przygotowana dla laika: prowadzi krok po kroku, ma wbudowaną pomoc po polsku i komunikaty w samej aplikacji. Nie wymaga instalacji, serwera ani konta. Nie wysyła żadnych danych do internetu.

> Aplikacja nie zawiera już trybu „pokoju wspomnień”. Zdjęcie pokoju z tego repozytorium możesz wykorzystać samodzielnie, bez aplikacji. Zobacz [Pokój wspomnień (bez aplikacji)](#pokój-wspomnień-bez-aplikacji).

### Funkcje
- **Działa z dowolnym AI.** To samo polecenie sprawdzi się w ChatGPT, Claude, Gemini, Grok, Copilot i innych. Model podpisuje się w danych, a aplikacja pokazuje, od którego AI pochodzą.
- **Ośmiu widoków wiedzy:** tożsamość, doświadczenie i droga, projekty, wiedza i kompetencje, umysł twórczy, oś czasu, wartości i wizja oraz interaktywna mapa powiązań (Canvas, z przeciąganiem, zoomem i obsługą klawiatury).
- **Uczciwe oznaczanie informacji.** Każdy wpis ma status (Fakt, Doświadczenie, Kompetencja, Osiągnięcie, Projekt, W trakcie, Koncepcja, Plan, Zainteresowanie, Wartość) i pewność (Pewne, Chyba prawda, Do sprawdzenia). Interpretacje AI są zawsze wyraźnie oznaczone jako **Domysł AI**.
- **Weryfikacja przez użytkownika.** Możesz odrzucać, przywracać i edytować wpisy, zanim uznasz uniwersum za swoje.
- **Wyszukiwarka** po całej bazie (klawisz `/`) i **pokaz na pełnym ekranie** (klawisz `P`).
- **Zapis jako plik HTML.** Aplikacja zapisuje samą siebie z Twoimi danymi w środku. Plik nazywa się `imie-ai-digital-universe.html` i otwiera się dwuklikiem, bez internetu. Jest też eksport samego JSON.
- **Przycisk „Nowe”** z przypomnieniem, że wynik nie został zapisany jako plik HTML. Wszystkie komunikaty są z aplikacji, nie systemowe.
- **Dostępność:** obsługa klawiatury, opcja ograniczenia ruchu (także zgodnie z ustawieniem systemu), responsywny układ.

### Stack technologiczny
- HTML5, CSS3, czysty JavaScript (bez frameworków i bez zależności).
- Canvas 2D (własny układ siłowy mapy powiązań).
- Dane w formacie JSON, przechowywane w `localStorage` przeglądarki i wbudowywane w zapisany plik HTML.
- Brak zewnętrznych bibliotek, czcionek i połączeń sieciowych.

### Wymagania
- Nowoczesna przeglądarka (Chrome, Edge, Firefox, Safari).
- Konto w wybranym asystencie AI z włączoną pamięcią (aplikacja podpowiada, jak to sprawdzić).

### Instalacja
Nic nie trzeba instalować. Pobierz plik:

```bash
git clone https://github.com/MrPrompt24/digital-universe.git
```

albo pobierz samo `digital-universe.html` z repozytorium.

### Uruchomienie
Otwórz `digital-universe.html` dwuklikiem. Działa bezpośrednio z dysku (`file://`), bez serwera lokalnego.

### Użycie
1. Na stronie startowej wpisz imię i wybierz swoje AI. Imię trafi do nazwy zapisywanego pliku.
2. Kliknij **Skopiuj polecenie** i wklej je w **nowym, zwykłym czacie** w swoim AI (nie w czacie tymczasowym, bo wtedy AI nie korzysta z pamięci).
3. Skopiuj całą odpowiedź (blok kodu zaczynający się od `{`) i wklej ją w aplikacji. Jeśli odpowiedź się urwie, napisz do AI „kontynuuj”.
4. W zakładce **Sprawdź dane** odrzuć to, co nieprawda, i popraw to, co niedokładne.
5. Przeglądaj sekcje, szukaj, użyj mapy powiązań.
6. W **Zapisz i ustawienia** zapisz wynik jako plik HTML. To Twoja kopia: otwórz ją dwuklikiem, kiedy zechcesz wrócić.

Zakładka **Pomoc** w aplikacji odpowiada na najczęstsze pytania (gdzie sprawdzić pamięć AI, co znaczą etykiety, co zrobić, gdy coś nie działa).

### Pokój wspomnień (bez aplikacji)
W repozytorium jest zdjęcie pustego pokoju: [`MrPromptRoom.png`](MrPromptRoom.png). Możesz go użyć samodzielnie, bez naszej aplikacji, żeby zobaczyć w formie obrazu, co AI o Tobie pamięta.

![Pusty pokój](MrPromptRoom.png)

**Jak to zrobić (w ChatGPT to działa):**
1. Pobierz obraz `MrPromptRoom.png` (zapisz lub skopiuj go).
2. Otwórz **nowy, zwykły czat** w ChatGPT. Nie używaj czatu tymczasowego.
3. Wklej obraz do czatu (Ctrl+V) albo dodaj go przyciskiem załącznika.
4. Napisz: **„Wypełnij ten pokój wszystkim, co o mnie wiesz”** i wyślij.
5. ChatGPT wygeneruje obraz pokoju umeblowanego rzeczami, których dowiedział się o Tobie z rozmów i pamięci.

**Dobrze wiedzieć:**
- W naszych próbach **obraz generuje ChatGPT**. Inne AI (np. Claude, Gemini) zwykle odpowiadają **tylko opisem**, bez obrazu.
- **Czat tymczasowy nie działa**, bo w ogóle nie korzysta z pamięci.
- Stopień zapełnienia zależy od tego, ile ChatGPT o Tobie wie. **Darmowe konto ma mniejszą pamięć**, więc pokój może wrócić pusty lub prawie pusty. To też jest wynik.
- Część rzeczy w pokoju może dotyczyć tego, o czym dawno zapomniano, albo czego nie chcesz, żeby było zapamiętane.
- Listę zapisanych wspomnień zobaczysz w ChatGPT: **Ustawienia → Personalizacja → Zarządzaj wspomnieniami**. Stamtąd możesz usunąć wspomnienia albo całkiem wyłączyć pamięć („Usuń i wyłącz pamięć”).
- **Usunięcie czatu nie usuwa tego, co ChatGPT z niego zapisał.** Trzeba usunąć samą pamięć.
- Na planach płatnych ChatGPT może korzystać także z poprzednich czatów, których nie ma na liście wspomnień.
- **Powtórz test za miesiąc** i porównaj oba pokoje obok siebie. Wszystko, co nowe na półkach, to coś, co AI dopisało w międzyczasie.

Zanim udostępnisz taki obraz komuś innemu, przejrzyj go: może pokazywać rzeczy prywatne.

### Format danych
Odpowiedź AI to JSON o strukturze `digital-universe/1`. Najważniejsze pola:

```json
{
  "schema": "digital-universe/1",
  "person": { "name": "", "headline": "", "summary": "", "self_definition": "" },
  "items": [
    {
      "id": "krotki-identyfikator",
      "kind": "project",
      "title": "nazwa",
      "summary": "1-3 zdania",
      "status": "projekt",
      "start": "2021-03",
      "end": "obecnie",
      "source": "pamięć / rozmowa / wniosek",
      "certainty": "potwierdzone",
      "tags": []
    }
  ],
  "relations": [{ "from": "id-a", "to": "id-b", "label": "używa" }],
  "gaps": ["czego AI o Tobie nie wie"],
  "meta": { "generated_by": "nazwa modelu", "generated_at": "RRRR-MM-DD", "memory_access": "" }
}
```

Dozwolone typy (`kind`): `fact`, `experience`, `achievement`, `event`, `project`, `organization`, `person`, `skill`, `technology`, `interest`, `idea`, `value`, `goal`. Pełny opis jest w poleceniu, które aplikacja kopiuje do schowka. Aplikacja sprawdza dane i po polsku wyjaśnia, co poprawiono lub pominięto.

### Prywatność
- Aplikacja nie ma serwera i nie wykonuje żadnych połączeń sieciowych. Dane zostają w przeglądarce oraz w plikach, które sam zapiszesz.
- To, co wkleisz do czatu z AI, trafia do firmy prowadzącej to AI, zgodnie z jej zasadami.
- **Nie publikuj** zapisanego pliku HTML z własnymi danymi w publicznym repozytorium: dane są wbudowane w środku pliku.
- Dane z AI to zbiór informacji o Tobie, które model mógł zapamiętać błędnie. Traktuj je jako punkt wyjścia i sprawdź w zakładce **Sprawdź dane**.

### Struktura projektu
```
digital-universe/
├── digital-universe.html   # cała aplikacja (HTML + CSS + JS) w jednym pliku
├── MrPromptRoom.png        # zdjęcie pustego pokoju do samodzielnego użycia w ChatGPT
├── README.md
└── LICENSE
```

### Testy
Projekt nie ma jeszcze zautomatyzowanych testów. Aplikację sprawdzano ręcznie w przeglądarce (wczytanie danych, weryfikacja, mapa, zapis i ponowne otwarcie pliku HTML). <!-- TODO: dodać testy automatyczne, jeśli projekt będzie rozwijany -->

### Współtworzenie
Zgłoszenia i propozycje są mile widziane:
1. Zgłoś błąd lub pomysł w [Issues](https://github.com/MrPrompt24/digital-universe/issues).
2. Zrób fork, wprowadź zmianę i otwórz Pull Request.

Aplikacja ma być **jednym plikiem HTML bez zależności i bez sieci**. Zmiany powinny to zachować.

### Licencja
Ten projekt jest objęty licencją MIT. Zobacz plik [LICENSE](LICENSE).

### Kontakt
**MrPrompt – Centrum Otwartych Innowacji**
Repozytorium: <https://github.com/MrPrompt24/digital-universe>

---

## 🇬🇧 English

### Table of Contents
- [About](#about)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Requirements](#requirements)
- [Installation](#installation)
- [Running the App](#running-the-app)
- [Usage](#usage)
- [Memory Room (without the app)](#memory-room-without-the-app)
- [Data Format](#data-format)
- [Privacy](#privacy)
- [Project Structure](#project-structure)
- [Tests](#tests)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

### About
AI assistants (ChatGPT, Claude, Gemini and others) remember details from your conversations. After many chats it is hard to know what exactly they know about you.

**Digital Universe** is a single-file HTML app that helps you see it:

1. you copy a ready-made prompt from the app and paste it into your AI,
2. the AI answers with structured data (JSON) describing what it knows about you,
3. you paste the answer into the app, which builds a readable dashboard: a connections map, timeline, projects, skills, values and goals.

The app is designed for non-technical users: it guides you step by step, has built-in help (in Polish) and in-app messages. No installation, server or account is needed. It sends no data to the internet.

> The app no longer includes a "memory room" mode. You can still use the room photo from this repository on your own, without the app. See [Memory Room (without the app)](#memory-room-without-the-app).

### Features
- **Works with any AI.** The same prompt works in ChatGPT, Claude, Gemini, Grok, Copilot and others. The model signs the data with its name, and the app shows which AI it came from.
- **Eight knowledge views:** identity, experience and journey, projects, knowledge and skills, creative mind, timeline, values and vision, and an interactive connections map (Canvas, with dragging, zoom and keyboard support).
- **Honest labeling.** Every entry has a status (Fact, Experience, Skill, Achievement, Project, In progress, Concept, Plan, Interest, Value) and a certainty level (Sure, Probably true, To check). AI interpretations are always clearly marked as **AI guess**.
- **User verification.** You can reject, restore and edit entries before you accept the universe as yours.
- **Search** across the whole knowledge base (key `/`) and a **full-screen presentation** (key `P`).
- **Save as an HTML file.** The app saves itself with your data embedded. The file is named `name-ai-digital-universe.html` and opens with a double click, offline. Plain JSON export is available too.
- **"New" button** with a reminder when the result has not been saved as an HTML file. All messages come from the app, not from the system.
- **Accessibility:** keyboard support, a reduced-motion option (also following the system setting), responsive layout.

### Tech Stack
- HTML5, CSS3, plain JavaScript (no frameworks, no dependencies).
- Canvas 2D (custom force-directed layout for the connections map).
- Data as JSON, kept in the browser's `localStorage` and embedded in the saved HTML file.
- No external libraries, fonts or network requests.

### Requirements
- A modern browser (Chrome, Edge, Firefox, Safari).
- An account with an AI assistant that has memory enabled (the app explains how to check).

### Installation
Nothing to install. Get the file:

```bash
git clone https://github.com/MrPrompt24/digital-universe.git
```

or download just `digital-universe.html` from the repository.

### Running the App
Open `digital-universe.html` with a double click. It works directly from disk (`file://`), no local server needed.

### Usage
1. On the start page enter your first name and pick your AI. The name is used in the saved file name.
2. Click **Copy prompt** and paste it in a **new, regular chat** in your AI (not a temporary chat, which does not use memory).
3. Copy the whole answer (a code block starting with `{`) and paste it into the app. If the answer is cut off, tell the AI to "continue".
4. In **Check data** reject what is untrue and fix what is inaccurate.
5. Browse the sections, search, use the connections map.
6. In **Save and settings** save the result as an HTML file. It is your backup: open it with a double click whenever you want to come back.

The in-app **Help** page answers common questions (where to check AI memory, what the labels mean, what to do when something fails).

### Memory Room (without the app)
The repository contains a photo of an empty room: [`MrPromptRoom.png`](MrPromptRoom.png). You can use it on your own, without our app, to see in the form of an image what an AI remembers about you.

![Empty room](MrPromptRoom.png)

**How to do it (this works in ChatGPT):**
1. Download the `MrPromptRoom.png` image (save or copy it).
2. Open a **new, regular chat** in ChatGPT. Do not use a temporary chat.
3. Paste the image into the chat (Ctrl+V) or attach it with the attachment button.
4. Type: **"Fill this room with everything you know about me"** (in Polish: *„Wypełnij ten pokój wszystkim, co o mnie wiesz”*) and send.
5. ChatGPT generates an image of the room furnished with things it learned about you from your chats and memory.

**Good to know:**
- In our tests **ChatGPT generates the image**. Other AIs (e.g. Claude, Gemini) usually answer **with a description only**, without an image.
- **A temporary chat will not work**, because it does not use memory at all.
- How full the room gets depends on how much ChatGPT knows about you. **A free account has less memory**, so the room may come back empty or almost empty. That is a result too.
- Some items may refer to things you mentioned long ago and forgot, or things you would rather not have remembered.
- You can see the saved memories in ChatGPT: **Settings → Personalization → Manage memories**. From there you can delete memories or turn memory off entirely ("Delete and turn off memory"). Menu names may differ by language and version.
- **Deleting a chat does not delete what ChatGPT saved from it.** You have to delete the memory itself.
- On paid plans ChatGPT may also use past chats that do not appear in the memory list.
- **Repeat the test in a month** and compare the two rooms side by side. Everything new on the shelves is something the AI has added in the meantime.

Before sharing such an image with anyone, review it: it may show private things.

### Data Format
The AI's answer is JSON with the `digital-universe/1` structure. Key fields:

```json
{
  "schema": "digital-universe/1",
  "person": { "name": "", "headline": "", "summary": "", "self_definition": "" },
  "items": [
    {
      "id": "short-identifier",
      "kind": "project",
      "title": "name",
      "summary": "1-3 sentences",
      "status": "projekt",
      "start": "2021-03",
      "end": "obecnie",
      "source": "memory / conversation / inference",
      "certainty": "potwierdzone",
      "tags": []
    }
  ],
  "relations": [{ "from": "id-a", "to": "id-b", "label": "uses" }],
  "gaps": ["what the AI does not know about you"],
  "meta": { "generated_by": "model name", "generated_at": "YYYY-MM-DD", "memory_access": "" }
}
```

Allowed `kind` values: `fact`, `experience`, `achievement`, `event`, `project`, `organization`, `person`, `skill`, `technology`, `interest`, `idea`, `value`, `goal`. The full description is in the prompt the app copies to your clipboard. Note that enumerated values such as `status` and `certainty` use Polish identifiers (e.g. `projekt`, `potwierdzone`, `obecnie`), as defined in that prompt. The app validates the data and explains (in Polish) what it fixed or skipped.

### Privacy
- The app has no server and makes no network requests. Data stays in your browser and in files you save yourself.
- What you paste into a chat with an AI goes to the company running that AI, under its policies.
- **Do not publish** a saved HTML file containing your own data in a public repository: the data is embedded inside the file.
- Data from an AI is a collection of things the model may have remembered incorrectly. Treat it as a starting point and verify it in **Check data**.

### Project Structure
```
digital-universe/
├── digital-universe.html   # the whole app (HTML + CSS + JS) in one file
├── MrPromptRoom.png        # empty room photo to use on your own in ChatGPT
├── README.md
└── LICENSE
```

### Tests
The project has no automated tests yet. The app has been checked manually in the browser (loading data, verification, the map, saving and reopening the HTML file). <!-- TODO: add automated tests if the project grows -->

### Contributing
Reports and suggestions are welcome:
1. Report a bug or an idea in [Issues](https://github.com/MrPrompt24/digital-universe/issues).
2. Fork the repo, make a change and open a Pull Request.

The app is meant to stay **a single HTML file with no dependencies and no network access**. Please keep it that way.

### License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

### Contact
**MrPrompt – Centrum Otwartych Innowacji**
Repository: <https://github.com/MrPrompt24/digital-universe>
