# boyu-timing.github.io
Stand 02.Feb.2023

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


Kannst du bitte mir helfen den Code zu ändern.
der aktuelle Code liegt in andere File "code Stand 02.Feb."
vielen Dank
