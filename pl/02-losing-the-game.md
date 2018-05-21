Pewnie zauważyłaś/-eś, że blok "przegrana" w skrypcie bohatera jest pusty. Zaraz go uzupełnisz i dodasz wszystkie potrzebne bloki aby stworzyć infromację o końcu gry.

1. Najpierw, uzupełnij blok "przegrana":   ![](/assets/losing1.bmp)

   * Zatrzymaj fizykę i wszystkie inne skrypty Bohatera
   * Powiedz wszystkim innym duszkom o końcu gry poprzez **nadanie komunikatu**
   * Przesuń Bohatera na środek ekranu i spraw by powiedział graczowi, że gra się skończyła

2. Teraz musisz się upewnić, że wszystkie duszki wiedzą co zrobić gdy gra się skończy i jak mają się zresetować gdy gracz postanowi rozpocząć nową grę. **Nie zapomnij o dodaniu tego skryptu do każdego duszka, którego dodasz gdy będziesz rozwijał/-a swoją grę!**

   Rozpocznij od tych łatwych duszków: "Platformy" i "Krawędzie". Oba te duszki muszą pojawiać się na początku gry i znikać na końcu.  ![](/assets/losing2.bmp)

3. Kolej na coś bardziej przebiegłego :-\). Jeżeli spojrzysz na kod dla duszka "Zbierane\_rzeczy" zauważysz, że **klonuje **sam siebie. Innymi słowy, tworzy kopie samego siebie a następnie wykonuje instrukcje podczepione do bloku "kiedy zaczynam jako klon".

   Będziemy mówić więcej co sprawia, że klony są wyjątkowe kiedy dotrzemy do karty sushi o robieniu nowych rzeczy do zbierania. Narazie, musisz wiedzieć, że klony mogą prawie wszystko to co standardowy duszek potrafi, właczając w to nadawanie komunikatów.

   Spójrzmy jak działa duszek "Zbierane\_rzeczy": ![](/assets/losing3.bmp)

   * Najpierw ukrywa oryginał duszka "Zbierane\_rzeczy"
   * Następnie ustawia wartość zmiennych sterujących. Wrócimy do tego później.
   * Zmienna "stwórz\_rzecz" włącza i wyłącza klonowanie: pętla tworzy klony jeżeli zmienna "stwórz\_rzecz" jest równa prawda. Jeżeli ta zmienna nie jest równa prawda pętla nie robi nic.

4. Teraz musisz stworzyć skrypt końca gry dla duszka "Zbierane\_rzeczy", podobny do tego jaki dodałaś/-eś do duszków "Krawędzie" i "Platformy". Jedyną różnicą jest fakt, iż należy zmienić wartość zmiennej "stwórz\_rzecz" na fałsz aby nowe klony rzeczy do zbierania się już nie tworzyły. Jest to przykład jak można wykorzystywać  zmienne aby nadać wiadomość z jednej części kodu do innego! ![](/assets/losing4.bmp)



