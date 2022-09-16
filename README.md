# Digitalizacja w systemach automatyki przemysłowej SIMATIC. Teoria, przykłady, ćwiczenia.
### Repozytorium stanowiące uzupełnienie do książki.
#### wyd. Helion, 2022


<img align="left" width="250px" src="/Images/DigiBook_Cover.png">
Droga użykowiczko, Drogi użytkowniku,

do Twojej dyspozycji oddaję specjalnie przygotowaną bibliotekę przykładów i gotowych projektów, dostępną w formie publicznego repozytorium. Choć większość przykładów i ćwiczeń opisywana jest dość szczegółowo w książce, każdy z nich przygotowany został w formie gotowych fragmentów kodu umieszczonych w przykładowym projekcie TIA Portal. Ponadto, część ćwiczeń w kolejnych rozdziałach książki realizowana jest w oparciu o funkcje opracowane na wcześniejszych stronach – wykorzystanie gotowego projektu pozwoli Ci więc zachować spójność i poprawną strukturę programu PLC, a także ułatwi realizację przykładów, które możesz oprzeć na gotowych szablonach.

------

W celu pobrania repozytorium na dysk twardy twojego komputera, możesz wykorzystać komendę dostepną w konsoli Git (system kontroli wersji musi być zainstalowany w Twoim systemie operacyjnym):
```
git clone https://github.com/newshade/Digitalizacja-w-systemach-automatyki.git
```
lub skorzystać z opcji pobrania plików w formie archiwum ZIP, oferowanej przez serwis GitHub:

![Pobieranie repozytorium za pomocą opcji Download ZIP](/Images/download_repo.png)

W części elementów dostępnych w repozytorium (m.in. przykładowym projekcie TIA Portal) nałozone zostało hasło dostępowe. Część wymaga również identyfikacji podając dodatkowo nazwę użytkownika. Wszędzie tam, gdzie niezbędne jest uwierzytelnienie, wykorzystywane są poniższe dane:
```
login: administrator
hasło: Sim@tic1518
```

------

### Digitalizacja

Choć jest to pojęcie powszechnie już znane i obecne w branży od kilku lat, wiele firm produkcyjnych czy przetwórczych nie rozpoczęło jeszcze wdrażania rozwiązań opisywanych ogólnie jako digitalizacyjne. Rozumiemy przez nie szereg zagadnień, których celem jest zmniejszenie przepaści pomiędzy obszarami operacyjnym i informatycznym, rządzącymi współczesnym światem.

> Praktyka pokazuje niestety, że choć otoczenie i technologie wokół nas pędzą naprzód niczym najnowszy model Ferrari, systemy stosowane w przemyśle możemy porównać raczej do przeciętnego auta klasy średniej. Choć działa bez zarzutu i wozi nas bezpiecznie z punktu A do B, nie zrobimy nim żadnego wrażenia pojawiając się na zlocie miłośników aut. Być może stracimy również możliwość nawiązania nowych kontaktów czy pozyskania klientów zainteresowanych przejażdżką.

> Ta analogia nie jest bezpodstawna – chcąc zachować konkurencyjność na rynku i móc oferować coraz lepsze produkty bądź usługi, niezbędne jest prowadzenie przedsiębiorstwa z duchem czasu, a nawet chęć wyprzedzenia konkurencji. W końcu jak powiedział kiedyś najbardziej utytułowany kanadyjski ho-keista Wayne Gretzky – Dobrego gracza poznaje się po tym, że zawsze jedzie tam gdzie akurat jest krążek. Wybitny zawodnik kieruje się tam, gdzie ten krążek będzie za chwilę.

------

### Wykaz odnośników w książce (odpowiedniki kodów QR):

#### Rozdział 3
- [View of Things - tworzenie prostych wizualizacji na poziomie serwera WWW wbudowanego w sterownik PLC SIMATIC](https://support.industry.siemens.com/cs/pl/en/view/109803395)

#### Rozdział 4
- [Dyrektywa Rady 2008/114/WE](http://data.europa.eu/eli/dir/2008/114/oj)
- [Wpis na stronie IEC n/t podziału IACS na strefy](https://gca.isa.org/blog/how-to-define-zones-and-conduits)
- [Omówienie komunikacji Open User Communication](https://support.industry.siemens.com/cs/ae/en/view/67196808)
- [Strona internetowa SiemensCERT](https://new.siemens.com/global/en/products/services/cert.html)

#### Rozdział 5
- [Praca z biblioteką projektu i bibliotekami globalnymi w TIA Portal](https://support.industry.siemens.com/cs/ww/en/view/109747503)
- [Porównywanie wersji bloków w bibliotece projektu w TIA Portal](https://support.industry.siemens.com/cs/ww/en/view/81748055)
- [Oficjalna strona systemu GIT - instalator](http://git-scm.com/downloads)
- [Versioc Control Interface (VCI) Git Connector - rozszerzenie do środowiska TIA Portal](https://support.industry.siemens.com/cs/ww/en/view/109773999)
- [Tworzenie nowego repozytorium w serwisie GitHub](https://docs.github.com/en/get-started/quickstart/create-a-repo)
- [Klient OPC UaExpert - instalator](https://www.unified-automation.com/products/development-tools/uaexpert.html)
- [Siemens OPC UA Modelling Editor - SiOME](https://support.industry.siemens.com/cs/ww/en/view/109755133)
- [Mosquitto Broker - instalator](https://mosquitto.org/download/)
- [Biblioteka LMQTT_Client dla sterowników PLC SIMATIC](https://support.industry.siemens.com/cs/ww/en/view/109780503)
- [Lista błędów i statusów HTTP](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status)
- [Mockoon - instalator](https://mockoon.com/download/)
- [Biblioteka LHTTP_Client dla sterowników PLC SIMATIC](https://support.industry.siemens.com/cs/ww/en/view/109780503)
- [Lista komend FTP](https://en.wikipedia.org/wiki/List_of_FTP_commands)
- [Biblioteka LFTP_Client dla sterowników PLC SIMATIC](https://support.industry.siemens.com/cs/ww/en/view/109780503)
- [Serwer FTP FileZilla - instalator](https://filezilla-project.org/download.php?type=server)
- [Biblioteka LStream dla sterowników PLC SIMATIC](https://support.industry.siemens.com/cs/ww/en/view/109781165)
- [Microsoft SQL Server Express - instalator](https://www.microsoft.com/pl-pl/sql-server/sql-server-downloads)
- [Microsoft SLQ Server Management Studio - instalator](https://docs.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms?redirectedfrom=MSDN&view=sql-server-ver16)
- [Tworzenie baz danych w Microsoft SQL Server](https://docs.microsoft.com/en-us/sql/relational-databases/databases/create-a-database?view=sql-server-ver16)
- [Omówienie składni języka SQL](https://www.w3schools.com/sql/default.asp)
- [Biblioteka LSQL_Client dla sterowników PLC SIMATIC](https://support.industry.siemens.com/cs/ww/en/view/109779336)

#### Rozdział 6
- [Obraz systemu na platformę SIMATIC IOT2050](https://support.industry.siemens.com/cs/ww/en/view/109741799)
- [Budowanie własnego obrazu systemu na platformę IOT2050](https://github.com/siemens/meta-iot2050)
- [Opis biblioteki node-s7-contrib dedykowanej dla środowiska Node-Red](https://flows.nodered.org/node/node-red-contrib-s7)

#### Rozdział 7
- [Platforma MindSphere - tworzenie darmowego konta](https://siemens.mindsphere.io/en/start)
- [OpenSSL - instalator](https://wiki.openssl.org/index.php/Binaries)

#### Rozdział 8
- [Aplikacja Performance Insight na panele HMI](https://support.industry.siemens.com/cs/ww/en/view/109780761)
- [Docker Desktop - instalator](https://docs.docker.com/desktop/windows/install/)
- [Dodatek WSL2 - instalator](https://docs.microsoft.com/pl-pl/windows/wsl/install-manual#step-4---download-the-linux-kernel-update-package)
- [Dokumentacja Docker-Compose](https://docs.docker.com/compose/compose-file/compose-file-v2/)
- [Przykład aplikacji wielokontenerowej do akwizycji i wizualizacji danych](https://github.com/newshade/DataAcquisition_Example)
