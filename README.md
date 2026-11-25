# Lord of the Board

<img src="icon-512.png" width="128" alt="Lord of the Board">

Snowboardowy **slalom gigant** w przeglądarce. Zjeżdżasz w dół stoku między bramkami i walczysz o jak najlepszy czas.

## Jak się jeździ
- **Start**: po odliczaniu stuknij **3 razy jak najszybciej**. Każde odepchnięcie dodaje prędkości, a im szybciej stukasz, tym mocniej się wybijasz (wynik w % widać po starcie).
- **Skręcanie**: przechylasz telefon w lewo i w prawo. Gra kalibruje się w czasie odliczania, więc trzymaj wtedy telefon tak, jak chcesz jechać prosto.
- **Fizyka jak w drifcie**: krawędź deski trzyma tylko do pewnej siły. Ostry skręt przy dużej prędkości kończy się poślizgiem bokiem (leci pył spod deski), a poślizg hamuje. Trzeba wyczuć, kiedy skręcić wcześniej i łagodniej.
- **Siatka**: wjedziesz w nią szybko i pod dużym kątem, to wypadasz z trasy i tracisz czas na powrót.
- **Bramki**: przejedź między dwoma słupkami. Ominięta bramka to **+3 s**.
- **Skoki**: na progu wybijasz się w powietrze. Skręt w locie obraca deskę, a lądować trzeba **wzdłuż kierunku jazdy** (tyłem też można). Krzywe lądowanie zabiera prędkość, bardzo krzywe kończy się upadkiem. Czysto wylądowany obrót daje bonus: **−0,5 s za każde 180°**.

## Tryby
- **Jazda solo**: trzy trasy (łatwa, średnia, trudna). Gra zapamiętuje rekord, a przy kolejnym przejeździe obok jedzie **duch** Twojego najlepszego zjazdu.
- **Dwóch graczy, jeden ekran (split screen)**: równoległy wyścig na tej samej trasie. Gracz 1 steruje klawiszami A/D i odpycha się W. Gracz 2 używa ←/→ i ↑. Na telefonie lub tablecie każdy gracz ma swoją połowę ekranu: przytrzymanie lewej albo prawej części skręca, a stukanie odpycha.
- **Online, dwa telefony**: jeden gracz tworzy pokój i wysyła link albo 4‑cyfrowy kod, drugi dołącza. Gospodarz wybiera trasę i startuje. Obaj jadą tę samą trasę naraz, a ekran jest podzielony: po lewej Ty, po prawej rywal na żywo (widać go też jako ducha na Twojej połówce). Liczy się czas razem z karami i bonusami. Po wyścigu jest **Rewanż** na nowej trasie.
  Połączenie działa jak w Gravity Ball: telefony łączą się jednocześnie przez trzy publiczne serwery MQTT po WebSocket (HiveMQ, EMQX i Mosquitto), więc gra działa w wifi i w sieci komórkowej, a awaria jednego serwera nie przerywa gry.

## Sterowanie na komputerze
←/→ albo A/D to skręt, spacja albo ↑ to odpychanie, a Esc lub P to pauza.

## Uruchomienie
Cała gra to jeden plik `index.html` bez zależności i bez budowania. Na GitHub Pages działa od razu (Settings → Pages → Deploy from branch). Na iPhonie dodaj stronę do ekranu początkowego, wtedy gra startuje na pełnym ekranie z ikoną. Przy pierwszym starcie iOS zapyta o dostęp do czujnika ruchu: zgódź się, bo bez tego skręcasz dotykiem.

Ikona jest w `icon.svg`, a pliki PNG (`icon-192.png`, `icon-512.png`, `apple-touch-icon.png`) są z niej wygenerowane.
