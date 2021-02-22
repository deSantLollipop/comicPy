# comicPy

nr.txt - plik z numerami indeksów komiksów które chciałbym zobaczyć na swojej stronie "index.html";
		 numery można dodawać i usuwać odpowiednio.

app.py - plik główny odpowiedzialny za pobieranie indeksów z pliku "nr.txt";
		 łączeniem i pobieraniem odpowiednich linków z https://xkcd.com/;
		 dodawanie "images" - listy pobranych linków, jako argumentu w funkcji render_template() - 
		 aby miec do niej dostęp z pliku index.html, dla kolejnych operacji;
		 odpalenie lokalnego hosta i strony "index.html", która jest domyślnie strona domowa.
		 Na stronie znajdują się zdjęcia, które można zobaczyć w całości po odpowiednim kliknięciu
		 przycisków pod zdjeciami - kliknicie przenosi bezpośrednio do oryginalnych linków każdego z obrazków.

base.html - bazowy html plik, szablon strony internetowej.

index.html - rozszerza plik "base.html", i jest go następcą. wtyczka z pythona:
			 w pętli dodaje kolejne elementy html klasy "card" do strony z odpowiednimi linkami na zdjęcia.
