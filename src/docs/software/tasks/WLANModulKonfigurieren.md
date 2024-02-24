# Konfiguration des WLAN Moduls
## Setup WLAN Tool

### Man Braucht:
- Laptop
- Admin account
- Ethernet Kabel
- POE Kabel

### 1: WLAN-Adapter anschliessen 

Als erstes muss der WLAN-Adapter richtig am Roboter installiert sein. Der Adapter hat zwei LAN Anschlüsse. Einer für LAN und Strom und der andere nur für LAN. Bei dem Anschluss welcher für LAN und Strom gedacht ist, muss man nun ein POE (Power Over Ethernet) Kabel anschliessen (oranges Kabel mit Verzweigung). Das eine Ende muss mit dem Laptop verbunden werden und das andere mit dem WLAN Adapter und der Stromquelle. Nun muss man noch mit einem zweitem LAN Kabel den zweiten Port mit dem Roborio verbinden.

### 2: Laptop konfigurieren

Nun muss man den Laptop von allen externen Verbindungen trennen, weil das Programm, welches man später benötigt, Probleme hat, den richtigen Port zu finden. Dafür muss man zuerst  die WLAN- und Buetooth-Verbindungen in den Einstellungen ausstellen. (Nur ausstellen über die Taskleiste funktioniert wahrscheinlich nicht!).

1. Öffne das Control Panel
2. Gehe zu *System and Secutiry*
3. Klicke auf der linken Seite auf *Network and Internet*
4. Klicke dann auf *Network and Sharing Center*
5. Klicke dann wider auf der linken Seite auf *Change adapter settings*
6. Nun sollten Dir die Bluetooth, Wi-Fi Verbindungen und vielleicht noch andere Verbindungen angezeigt werden. Mit der rechten Maustaste kann man sich die Optionen anzeigen lassen. Wähle bei allen Verbindungen, ausser die Ethernet Verbindung,  *disable* aus um die Verbindung zu stoppen. (Dafür benötigt man das Admin Passwort)

Nun müssen wir noch die Firewall ausstellen. Dies wird wie folgt gemacht.
1. Gehe wieder zu den *System and Security* Einstellugen.
2. Klicke auf der rechten Seite auf *Windows Defender Firewall*
3. Klicke dann auf der linken Seite auf *Turn Windows Defender Firewall on or off* um die Firewall auszustellen. (Dafür wird wieder das Admin Passwort benötigt).

### 3: WLAN Tool Einrichten

Nun kann man mit dem eigetlichem Einrichten beginnen.
Dafür braucht man zwei Tools. Zum einen das FRC Radio Configuration Utility Tool, und zum anderm das Roborio Team Number Setter.  

Öffne zuerst das FRC Radio Configuration Utility Tool. (Wieder admin..). Es sollte ein Pop Up erscheinen, wo man *Ethernet..* auswählen muss.

1. Die Daten sollten eingegeben werden:
    - Team number (Wichtig)
    - Name
    - Die anderen Felder können auf der Standarteinstellung gelassen werden.

2. Load Firmware:
    - Klicke zuerst auf Load Firmware und warte bis auf dem Fenster etwas wie „Powsercycle“ steht
    - Wenn diese Nachricht gekommen ist, ziehe das LAN Kabel am WLAN Adapter welches die Verbindung zum Laptop hat, kurz aus. Danach muss man es wieder einstecken. Und danach warten bis es beendet ist. 

3. Configure
    - Als zweites kann man versuchen den WLAN Adapter konfigurieren.
    - Zuerst entferne die Verbindung zum WLAN Adapter zum Roborio.
    - Danach klicke auf Configure und warte.
    - Wenn kein Fehler kommt kann man zu Schritt vier gehen. Kommt eine Fehlermeldung, dann gehe zu Schritt vier und dann versuche Schritt drei noch einmal. 

4. Set Team Number
    - Öffne für diesen Schritt das *Roborio Team Setter Tool*. Gebe danach die Team Number ein und klicke auf *set*.
    - Danach sollte der WLAN Adapter eigentlich funktionieren. Um dies zu testen, öffnen die Driverstation und schaue ob eine Verbindung zustande kommt.
    - Wenn es nicht funktioniert, dann muss man einfach ausprobieren und hoffen das es funktioniert x_x.



