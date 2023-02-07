# boyu-timing.github.io
Stand 07.Feb.2023

Lieber Martin,
Hier ist mein neu User Experience

ich hätte gerne jetzt LED blinken statt fade, da die neue Situation kompliziert ist. Mit blinken kann man schnell die Änderung sehen.
kannst du bitte neuer Code erst trotzdem auf Ultraschall Sensor basieren, damit ich die Daten selber testen kann?
Wenn alles gut funktioniert, tauschen wir den Code nachher dann zu lidar sensor.



<Abstand weniger als 30 cm>: Servomotor in 0 Grad , LED komplett aus

<Abstand von 30-100 cm>:

Situation 1: Wenn eine Person sich dem Gerät langsam nähert oder sich von ihm entfernt (Abstand ändert sich weniger als 10cm pro 500ms), wird der Servomotor im Stillstand bleiben (egal in welchem Winkel er sich vorher befand.) Wenn die Person weit weg ist, blinkt das LED langsam, wenn die Person nah ist, blinkt das LED schnell.

Situation 2: Wenn eine Person sich etwas schnell dem Gerät nähert oder sich von ihm entfernt (Abstand ändert sich mehr als 10cm pro 500ms.),

Servomotor: Wenn sich der Abstand um 1 cm ändert, dreht sich der Servomotor um 2 Grad. (sieht Code unten, das kann man evtl. weiter verwenden)

Aktuelle Servomotor Code: myservo.write(map(cm,30,100,40,180));

LED: Wenn die Person weit weg ist, blinkt das LED langsam, wenn die Person nah ist, blinkt das LED schnell.

Situation 3: Wenn eine Person sich sehr schnell dem Gerät nähert oder sich von ihm entfernt (Abstand ändert sich mehr als 40cm pro 500ms.), dreht der Servomotor direkt bis 0 Grad, regal in welchem Winkel das Motor vorher war. LED komplett aus.

<Abstand mehr als 100cm>: Servo Motor in 180 Grad , LED komplett aus



repeat again in english

If the distance is less than 30cm, the servo motor will be set to 0 degrees and the LED will be turned off. 

If the distance is between 30-100cm, there are three different situations:

1. If the distance changes by less than 10cm per 500ms, the servo motor will not move and the LED will blink either slowly or fast based on the distance.(long distance blink slowly, short distance blink quickly)

2. If the distance changes by more than 10cm per 500ms, the servo motor will rotate by 2 degrees for every 1cm change in distance and the LED will blink either slowly or fast based on the distance.
3. If the distance changes by more than 40cm per 500ms, the servo motor will immediately turn to 0 degrees, regardless of its previous position, and the LED will be turned off.

If the distance is more than 100cm, the servo motor will be set to 180 degrees and the LED will be turned off.


Kannst du bitte mir helfen den Code zu ändern.
der aktuelle Code liegt in andere File "code Stand 02.Feb."
vielen Dank
