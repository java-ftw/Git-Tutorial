# Konfiguracja podstawowa

# 1. Twoja tożsamość
Pierwszą rzeczą, którą warto wykonać po instalacji Git jest konfiguracja własnej nazwy użytkownika oraz adresu e-mail. Jest to ważne, ponieważ każda operacja zatwierdzenia w Git korzysta z tych informacji, które stają się integralną częścią zatwierdzeń przesyłanych i pobieranych później do i z serwera:

		
		$ git config --global user.name "Jan Nowak"
		
		Nazwa ma być zbliżona do naszej oryginalnej nazwy użytkowania na Githubie
		
		$ git config --global user.email jannowak@example.com
		
		Używamy tutaj swojego oryginalnego maila z jakim zostanie połączone nasze konto na GitHubie

# 2. Edytor
Teraz, gdy ustaliłeś swą tożsamość, możesz skonfigurować domyślny edytor tekstu, który zostanie uruchomiony, gdy Git będzie wymagał wprowadzenia jakiejś informacji tekstowej. Domyślnie Git skorzysta z domyślnego edytora systemowego, którym zazwyczaj jest Vi lub Vim. Jeśli wolisz korzystać z innego edytora, np. z Emacsa, uruchom następujące polecenie:

	$ git config --global core.editor emacs
	
	Ustawiamy edytor który nam pozwoli edytować oraz jest wygodny dla uzytkownika

# 3. Narzędzie obsługi różnic
Warto również skonfigurować domyślne narzędzie do rozstrzygania różnic i problemów podczas edycji konfliktów powstałych w czasie operacji łączenia (ang. merge). Jeśli chcesz wykorzystywać w tym celu narzędzie vimdiff, użyj polecenia:

	$ git config --global merge.tool vimdiff

# 4.Sprawdzamy ustawienia

Warto też sprawdzić bieżące ustawienia wykonujemy je za pomocą: 

	$ git config --list
	user.name=Scott Chacon
	user.email=schacon@gmail.com
	color.status=auto
	color.branch=auto
	color.interactive=auto
	color.diff=auto

Możemy również sprawdzić konkretną zmienną za pomocą komendy: 
	
	$ git config user.name
	Scott Chacon
