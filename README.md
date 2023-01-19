# boyu-timing.github.io
all about timing code

Lieber Martin,
ich habe meine Code von Abstand Sensor hochgeladen (File:Abstand Sensor code ). 
Ich brauche auch die LED Panel und den Servomotor zu ändern, je nach den Daten aus dem Abstandssensor.

Ich brauche folgende Hilfe bei Coding von Ihnen:

Abstandsensor Code: Der Sensor misst nur Daten zwischen 0 und 180 cm. Andere Daten werden ignoriert.

Servo Motor Code: Der Drehwinkel des Servomotors ist auf 0 bis 180 Grad begrenzt. Der Winkel des Servomotors entspricht dem vom Abstandssensor gemessenen Wert, z. B. wenn die Person 50 cm vom Sensor entfernt ist, beträgt der Winkel des Servomotors 50 Grad. Bei einer Entfernung von 180 cm beträgt der Winkel 180 Grad. Der Winkel wird pro 1 cm Abstand zwischen der Person und dem Abstandssensor um 1 Grad verringert. 

Servo Motor Code besondere Timing: Der Servomotor dreht sich so schnell wie möglich auf 0 Grad, wenn sich eine Person weniger als 20 cm vom Sensor entfernt befindet.

Led Code:Das LED-Licht schaltet sich nicht ein, wenn der Sensor eine Person in einer Entfernung von mehr als 180 cm erkennt. Bei einer Entfernung von weniger als 180 cm beginnt das LED-Licht langsam zu verblassen(fading). Je geringer der Abstand zwischen der Person und dem Sensor wird, desto schneller wird das Licht verblassen(fading). Wenn der Servomotor auf 0 Grad dreht, erreicht die Fading-frequenz ihr Maximum.

vielen Dank
mit besten Grüßen
boyu
