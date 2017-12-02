1. To są karty Sushi z zadaniem na zaawansowanym poziomie Scratcha. Pracując z nimi będziesz tworzyć grę platformową, do której będziesz mógł dodawać swoje poziomy, power-upy i bohaterów.

   ![](assets/setup1.png)

2. Ponieważ uczysz się Scratcha a nie jak zbudować silnik oparty na fizyce \(kod, który sprawia, że rzeczy "zachowują się" jak w rzeczywistości, np. nie  przelatują przez ściany czy podłogi\), zaczniesz projekt kopiując gotowy skrypt, który zawiera podstawowe ruchy, skakanie i wykrywanie platform.

   Spójrz na ten skrypt gdyż później będziesz dokonywał w nich zmian jednak nie musisz rozumieć wszystkiego co skrypt wykonuje.

3. Pierwszym krokiem jest skopiowanie skryptu z projektu [dojo.soy/advanced-scratch](http://dojo.soy/advanced-scratch).

   Możesz pobrać ten skrypt klikając "Zajrzyj do środka", następnie **Plik **w pasku zadań, wybierz "Pobierz na swój komputer", a na końcu otwórz ten projekt na swoim komputerze.

   Możesz użyć projekt bezpośrednio w swojej przeglądarce klikając "Zajrzyj do środka", a następnie "Remiks".

4. Silnik fizyki gry składa się z różnorodnych części. Niektóre z nich już działają na tym etapie, a niektóre nie. Działanie skryptów możesz sprawdzić uruchamiając grę i próbując w nią zagrać.

   Możesz tracić życia ale nic się nie dzieje jeśli stracisz je wszystkie. Ponadto, gra ma tylko jeden poziom, jeden typ rzeczy, które można zebrać i nie ma przeciwników. Naprawisz to wszystko i zrobisz jeszcze więcej!

   Teraz, spójrz jak skrypty są połączone ze sobą. Użyto zostało wiele **"Więcej bloków"**, które można podzielić na mniejsze, bardziej zrozumiałe części. To jak mieć jeden blok stworzony z wielu innych podstawowych bloków.

   ![](/assets/image3379.png)

   * Główna pętla gry - pętla zawsze wywołuje blok główna fizyka, który wykonuje wiele rzeczy! Gdy mamy je osobno skrypt jest przejrzystszy, bardziej czytelny i łatwiej zrozumieć co się **kiedy **dzieje nie martwiąc się **jak **to się dzieje.

5. Teraz spójrz na Now look at `reset game` and `reset character` and notice:

   * They do pretty normal things—setting up variables, making sure the character rotates properly
   * `reset-game` **calls** `reset-character`—you can use a **more block** inside another **more block**!
   * `reset-character` gets used in two different places, but to change it you only have to change the code of the **more block** in one! This can save you a lot of work and help you avoid mistakes.



