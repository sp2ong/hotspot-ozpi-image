Eksperymentalny obraz FM POLAND **Orange PI Zero v1.x**

( Obraz dla Orange Pi Zero **v3** znajdziesz tu:  https://github.com/radioprj/orangepizerov3/releases/tag/v1.0 )

( Obraz dla Raspberry PI znajdziesz tu: https://github.com/FM-POLAND/hotspot-rpi-image/releases/tag/1.0 )

Obraz przeznaczony do budowy hotspota domowego z wykorzystaniem modułu radiowego SA818

Obraz o nazwie **fmpoland-ozpi.img.xz** nagrać na kartę microSD (8 Gb lub większa) przy pomocy: https://etcher.balena.io/

Login do konsoli via ssh:

user: root

hasło: fmpoland

Zalecana zmiana hasła poleceniem: **passwd**

Dostęp do dashboard:

http://hotspot-fmpl.local/

lub

http://ip_adres

IP adres możesz znaleźć przy pomocy darmowego narzędzia: https://www.advanced-ip-scanner.com/pl/

Konfiguracja via Dashboard, należy wybrać z menu "Admin" i następnie: 

W pierwszej kolejności sprawdź poprawne ustawienia obsługi SQL i PTT w menu

**SQL PTT"

Po sprawdzeniu / ustawieniu  SQL / PTT dopiero wtedy możesz przejść do konfiguracji:

"SVXCnf" - konfiguracja konta FM POLAND

"NodeInfo" - Informacje o stacji

"WEBCnf" - konfiguracja Dashboard

oraz inne opcje stosownie do potrzeb

CZYTAJ uważnie informacje umieszczone w każdym oknie z serii administracyjnych
w których są istotne informacje do dostępnych ustawień

![Admin Menu](https://github.com/sp2ong/hotspot-ozpi-image/blob/main/admin-menu.png)

Domyślnie obraz przygotowany do pracy z płytkami radiowymi SA818/SA868 na bazie schematu SPOTNIK lub ROLINK


Można wykorzystać obraz z dowolnym radiem np GMxx, BF-888, UVK5, UV5R itp podłączając go: http://fm-poland.pl/schemat-intrefejsu-dla-orange-pi-zero-anyradio/


Jeśli dashboard będzie dostępny z zewnątrz (zastanów sie czy jest to ci niezbędne)  to aby dostać się do menu ADMIN należy w Admin -> WebCnf w opcji REMOTEIP zamiast adresu 127.0.0.1 wpisać zdalny zaufany IP adres (ZALECANE: można skorzystać z VPN [Tailscale](https://tailscale.com/) wersja personal zawiera darmową obsługę 3 userów/100 urządzeń). Można też dostać z publicznego adresu do strony dashboard po linkiem

http://ipadresdashboard/svxc/

po podaniu użytkownika i hasła gdzie można wyłączyć lub włączyć zdalnie odbiornik SVXLINK. Jak założyć użytkownika i dla niego hasło patrz opis na swoim hotspot w pliku /etc/svxlink/SVXControl.txt

![Hotspot login](https://github.com/sp2ong/hotspot-ozpi-image/blob/main/hotspot-login.png)

Obraz zawiera dwa rodzaje dashboard, Domyślny w wersji "BLUE" stary dashboard tzw "jasny"

**Eksperymentalny obraz używasz na własną odpowiedzialność i autor nie ponosi odpowiedzialności za wykorzystane rozwiązanie i wynikające z niego skutki.**
.
