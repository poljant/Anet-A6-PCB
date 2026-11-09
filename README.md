# Anet-A6-PCB
Przystosowanie drukarki 3D Anet A6 do tworzenia PCB.

PenHolder został utworzony za pomocą prgramu FreeCAD.
Projekt ten znajduje się w katalogu FreeCAD.
PenHolder składa się z pięciu części wydrukowanych na drukarce 3D, oraz szyn wykonanych z pręta aluminiowego o średnicy 5mm.
Pliki drukowałem z Pet-G.

Zasada działania;
Na szynach jest umieszczony suwak, który trzyma pisak. W moim przypadku otwór dla pisaka jest 10mm. Jakby pisak był cieńszy to można do owinąć taśmą. Grubszy też może być, bo długość śrub na to pozwala.
Suwak swobodnie przemieszcza sie góra dół, pod własnym ciężarem. Po wydruku i zmontowaniu holderu należy przesuwać nim tak długo aż suwak będzie poruszał się swobodnie bez oporu ale nie za luźno bo dokładność drukowania się pogorszy.
Ciężar suwaka (suwak z nasadką suwaka i śruby z nakrętkami motylkowymi) i pisaka jest wystarczajacy do prawidłowego pisania na płytce PCB. Gdyby okazało się, że nacisk jest zbyt mały, to pisak można dociążyć dodatkowym ciężarkiem. Ja nie miałem takiej potrzeby, dla pisaków 0.4 i 0.6mm.
Zestaw podzielony jest na pięć części, aby otwory dla pręta 5mm, drukować na płasko (część górna i dolna).
Suwak jest drukowany od dołu do góry (wg zamocowania), aby otwory dla pręta były drukowanie w pionie.
Dolna i górna część podstawy przykręcone są śrubami 3mm.
Nasadka jest przykręcona do suwaka śrubami 3mm z nakrętkami motylkowymi (łatwa wymiana pisaka).
Pliki *.stl zawierają wszystkie części potrzebne do zrobienia uchwytu pisaka, nazwa pliku określa nazwę części.

Płytkę PCB zrobiłem w KiCAD. W nim utworzyłęm pliki GERBER.
Do tworzenia plików *.gcode z plików GERBER, które sterują drukowaniem PCB zastosowałem program FlatCAM.
Należy ustawić średnicę pisaka, szybkość druku (400, szybkość przemieszczania 120).
Przy szybkości 500 tusz nie rozpływał się dobrze.
Poziom Z przemieszczania na 3mm.
Poziom pisania ustaw na Z-1mmm.
Drukowałem pisakiem 0.6 i 0.4, krycie tuszem jest bardzo dobre.

Gdy drukarka stanie na pozycji drukowania, to należy ustawić pisak tak aby swobodnie dotykał PCB.
Pisak należy ustawić 1mm wyżej od pozycji minimalnej na suwaku, aby swobodnie naciskał na płytkę PCB i nie opierał się dolną cześć podstawy.
Jeśli przy większych PCB są problemy z poziomowaniem stoły drukarki, to suwak z pisakiem można ustawiś wyżej niż 1mm od podstawy holdera.

W pliku *.gcode dla drukarki Anet A6 i dla tego holdera, należy ustawić kody od pierwszego do M3.
Kody te są zawarte w pliku gcode.txt. Wystarczy skopiować zawartość pliku do początku pliku *.gcode.

