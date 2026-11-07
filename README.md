# Anet-A6-PCB
Przystosowanie drukarki 3D Anet A6 do tworzenia PCB.

PenHolder składa się z pięciu części wydrukowanych na drukarce 3D, oraz szyn wykonanych z preta aluminiowego o średnicy 5mm.
Pliki drukowane są z Pet-G.
zasada działania;
Na szynach jest umieszczony suwak, który trzyma pisak. 
Suwak swobodnie przemieszcza sie góra dół, pod własnym ciężarem.
Ciężar suwaka i pisaka jest wystarczajacy do prawidłowego pisania na płytce PCB. Gdyby okazało się, że nacisk jest zamały, to pisak można dociążyć dodatkowym ciężarkiem. Ja nie miałem takiej potrzeby, dla pisaków 0.4 i 0.6mm.
Zestaw podzielony jest na pięć części, aby otwory dla pręta 5mm, drukować na płasko (część górna i dolna.
Suwak jest drukowany od dołu do góry (wg zamocowania), aby otwory dla pręta były drukowanie w pionie.
Dolna i górna część podstawy przykręcone są śróbami 3mm.
Nasadka jest przykręcona do suwaka śrubami 3mm z nakretkami motylkowymi (łatwa wymiana pisaka.
Pliki *.stl zawierają wszystkie części potrzebne do zrobienia uchwytu pisaka, nazwa pliku określa jaka to część.

Płytkę PCB zrobiłem w KiCAD. W nim utworzyłęm pliki GERBER.
Do tworzenia plików *.gcode z plików GERBER, które sterują drukowaniem PCB zastosowałem program FlatCAM.
Należy ustawić średnicę pisaka, szybkość druku (400, szybkość przemieszczania 120).
Przy szybkości 500 tusz nie rozpływał się dobrze.
Poziom Z przemieszczania na 3mm.
Poziom pisania ustaw na Z-1mmm.
Drukowałem pisakiem 0.6 i 0.4, krycie tuszem jest bardzo dobre.

Pisak należy ustawić 1mm wyżej od pozycji minimalnej na suwaku, aby swobodnie naciskał na płytkę PCB.
Gdy drukarka stanie na pozycji drukowania, to należy ustawić pisak tak aby swobodnie dotykał PCB.

