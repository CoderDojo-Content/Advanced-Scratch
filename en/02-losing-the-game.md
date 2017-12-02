1. Pewnie zauważyłaś/-eś, że blok "przegrana" w skrypcie bohatera jest pusty. Zaraz go uzupełnisz i dodasz wszystkie potrzebne bloki aby stworzyć infromację o końcu gry.

   Najpierw, uzupełnij blok "przegrana":   ![](/assets/ScreenHunter_003.bmp)

   * Zatrzymaj fizykę i wszystkie inne skrypty Bohatera
   * Powiedz wszystkim innym duszkom o końcu gry poprzez **nadanie komunikatu**
   * Przesuń Bohatera na środek ekranu i spraw by powiedział graczowi, że gra się skończyła

2. Teraz musisz się upewnić, że wszystkie duszki wiedzą co zrobić gdy gra się skończy i jak mają się zresetować gdy gracz postanowi rozpocząć nową grę. **Nie zapomnij o dodaniu tego skryptu do każdego duszka, którego dodasz gdy będziesz rozwijał/-a swoją grę!**

   Rozpocznij od tych łatwych duszków: "Platformy" i "Krawędzie". Oba te duszki muszą pojawiać się na początku gry i znikać na końcu.  ![](/assets/ScreenHunter_004.bmp)

3. Kolej na coś bardziej przebiegłego :-\). Jeżeli spojrzysz na kod dla duszka "Zbierane\_rzeczy" zauważysz, że **klonuje **sam siebie. Innymi słowy, tworzy kopie samego siebie a następnie wykonuje instrukcje podczepione do bloku "kiedy zaczynam jako klon".

   Będziemy mówić więcej co sprawia, że klony są wyjątkowe kiedy dotrzemy do karty sushi o robieniu nowych rzeczy do zbierania. Narazie, musisz wiedzieć, że klony mogą prawie wszystko to co standardowy duszek potrafi, właczając w to nadawanie komunikatów.

   Spójrzmy jak działa duszek "Zbierane\_rzeczy": ![](/assets/ScreenHunter_008.bmp)

   * Najpierw ukrywa oryginał duszka "Zbierane\_rzeczy"
   * Następnie ustawia wartość zmiennych sterujących. Wrócimy do tego później.
   * The `create-collectables` variable is the on/off switch for cloning: the loop creates clones if `create-collectables` is `true`, and does nothing if it’s not

4. Now what you need to do is setup a block like the ones you had on the “Edges” and “Platforms” sprites on the “Collectable” sprite. The only difference is you’re also setting the `create-collectables` variable to `false` so that no new clones are created. Notice how you can use the variable to pass messages from one part of your code to another! ![](assets/losing4.png)



