#  Słownik


-  **SCM**  – to akronim od Source Code Management, czyli dosłownie kontrola kodu (w języku polskim funkcjonuje określenie system kontroli wersji); jest to system który pozwala na archiwizowanie i śledzenie zmian w kodzie, dzięki czemu możemy cofać się w historii lub podejrzeć, kto był autorem konkretnej zmiany

- **Repozytorium** – ‚kontener’ na określony zbiór kodu, najczęściej jeden projekt; repozytorium pozwala grupować kod i zmiany, dzięki czemu możemy przeglądać wszystkie zmiany wykonane w ramach jednego repozytorium, przyznawać uprawnienia do repozytoriów oraz pobierać / kopiować je

- **Commit (lub rewizja)** – jest to proces ‚wysłania’ na repozytorium określonych zmian w kodzie – jeśli pobierasz kod z repozytorium, następnie dokonujesz modyfikacji i wysyłasz te zmiany z powrotem do repozytorium, proces ten nosi nazwę commitowania, a same zmiany wysłane razem nazywamy commitem lub rewizją

- **pull / push** – odpowiednio pobranie i wysłanie zmian (jednego lub wielu commitów) z/do innego repozytorium

- **diff – (ang. różnica)** – jest to różnica pomiędzy różnymi rewizjami – dzięki temu możemy zobaczyć, które fragmenty uległy zmianie oraz w jaki sposób; pozwala to także zoptymalizować transfer danych pomiędzy repozytoriami

- **fork** – kopia repozytorium; szczególnie popularne w przypadku projektów open-source, dzięki czemu możemy skopiować cały projekt i rozwijać go niezależnie (np. dopasowując do naszych potrzeb)

- **branch** – odgałęzienie, wersja wewnątrz repozytorium; branche pozwalają na prace wielu osobom równocześnie, bez ciągłego wchodzenia sobie w drogę i nadpisywania zmian – każdy może pracować na swoim branchu, dopiero po zakończeniu pracy łącząc zmiany z innymi i rozwiązując problemy

- **merge** – połączenie wielu zmian z różnych źródeł, które może skutkować niekompatybilnymi zmianami wymagającymi ręcznych modyfikacji; merge pozwala łączyć prace wykonywane w różnych obszarach, które mogą się zazębiać, w jedną całość w sposób kontrolowany i świadomy

# Tutaj więcej super komend, które nam pomogą 

- **git init** 
 Inicjalizuje repozytorium GIT w danym katalogu
- **git add [nazwa_pliku]**
Dodaje zmiany we wskazanym pliku do commita
- **git add .**
Dodaje wszystkie zmienione pliki do commita
- **git add -p [nazwa_pliku]**
Udostępnia możliwość dodania wybranych linii w zmodyfikowanym pliku do commita
- **git commit -m "[treść_commita]"**
Dodaje opis do commita. Dobrym zwyczajem jest opisanie co ta zmiana wprowadza do kodu w zakresie funkcjonalnym
- **git add origin [adres_repozytorium, np. https://github.com/username/moje-repozytorium.git]**
Ustawia konkretny adres zdalnego repozytorium jako główne repozytorium
- **git push origin master**
Wysłanie zmian do branacha zdalnego
- **git push -f**
Wysłanie zmian do zdalnego repozytorium ignorując konflikty, to znaczy, że jeśli wystapią konflikty to pliki zostaną nadpisane właśnie wysłaną wersją. Trzeba stosować to bardzo ostrożnie.
- **git checkout [nazwa_brancha]**
Zmienia aktywny branch na wybrany przez użytkownika
- **git checkout [nazwa_pliku]**
Usuwa zmiany w wybranym pliku
- **git checkout .**
Usuwa zmiany we wszystkich zmienionych plikach
- **git checkout -b [nazwa_brancha]**
Tworzenie nowego brancha z aktywnego brancha i przełączenie się na niego
- **git rebase master**
Zaciągnięcie zmian z brancha głównego do brancha aktywnego
- **git push origin :[nazwa_brancha**]
Usunięcie zdalnego brancha
- **git branch -d [nazwa_brancha]**
Usuwanie brancha lokalnie. Nie można usunąć w ten sposób aktywnego brancha
- **git stash**
Dodanie zmienonych plików do pamięci/stosu i usunięcie ich z aktywnego brancha
- **git pull --rebase**
Pobranie najnowszych zmian z aktywnego brancha zdalnego
- **git stash pop**
Przywrócenie zmodyfikowanych plików z pamięci/stosu
- **git stash clear**
Czyszczenie pamięci/stosu
- **git remote prune origin**
Pobranie aktualizacji o usuniętych branchach zdalnych
- **git fetch --all**
Pobranie listy zdalnych branchy
- **git branch**
Wyświetlenie listy lokalnych branchy
- **git branch -r**
Wyświetlenie listy zdalnych branchy
- **git status**
Wyświetlenie listy zmienionych plików
- **git diff [nazwa_pliku]**
Szczegółowe wyświetlenie zmian w wybranym pliku
- **git reset HEAD**
Resetowanie przygotowanych commitów (przed wysłaniem). Zmodyfikowane pliki są dostępne do ponownego dodania.
- **git reset HEAD --hard**
usuwanie wszystkich zmian z brancha lokalnego i przywrócenie zmian z brancha zdalnego
- **git reset HEAD^ --hard**
Usuwanie ostatniego commita z brancha
- **git reset HEAD^^**
- **git reset HEAD~2**
Obydwie komendy usuwają ostatnie 2 zmiany z brancha. Im więcej daszków (^) tym więcej commitów zostanie usuniętych.
- **git rebase -i HEAD~3**
Interaktywne zmienianie zawartości, opisów commitów. Commity mozna łączyć wtedy w jeden duży, zmienić jego opis, itd.

# Kilka przydatnych komend do obsługi "Markdown"

### Welcome to MarkdownPad 2 ###

**MarkdownPad** is a full-featured Markdown editor for Windows.

### Built exclusively for Markdown ###

Enjoy first-class Markdown support with easy access to  Markdown syntax and convenient keyboard shortcuts.

Give them a try:

- **Bold** (`Ctrl+B`) and *Italic* (`Ctrl+I`)
- Quotes (`Ctrl+Q`)
- Code blocks (`Ctrl+K`)
- Headings 1, 2, 3 (`Ctrl+1`, `Ctrl+2`, `Ctrl+3`)
- Lists (`Ctrl+U` and `Ctrl+Shift+O`)

### See your changes instantly with LivePreview ###

Don't guess if your [hyperlink syntax](http://markdownpad.com) is correct; LivePreview will show you exactly what your document looks like every time you press a key.

