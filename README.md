# docker-compose-LAMP-lab


Aplikacja wyświetlająca jednolinijkowy skrypt php: <>php phpinfo(); ?>
Ze względu na użycie linkowania kontener z bazą danych mysql startuje jako pierwszy, dopiero w momencie sygnału o starcie uruchomiony zostaje kontener php.

Do połączenia katalogu DocumentRoot przechowujący skrypt z katalogiem wewnetrznym kontenera został zamontowany volumen typu bind.
Kontener php został wystawiony pod adresem: localhost:80
Natomiast kontener httpd pod adresem: localhost:6666

Wszystkie kontenery zostały podłączone do utworzonej sieci "backend"
Kontener httpd dodatkowo został podłączony do sieci "frontend"

