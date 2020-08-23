# Spieler Management

Gamemode:
   Der Spieler Gamemode kann ganz einfach gesetzt
   werden. Die Zahl zwischen den `()` zeigt
   den Gamemode, inden der Spieler gesetzt werden
   soll ;)
   ```php
      $player->setGamemode(1);
   ```
Kicken:
   Um Spieler zukicken, gibt es 2 verschiedene
   möglichkeiten.
   Variante 1:
   ```php
   $player->kick($grund);
   ```
   Variante 2:
   ```php
   $player->close($grund);
   ```
Bannen:
   Um Spieler zubannen, gibt es eine Art, aber 
   viele würden es falsch machen. Die meisten würden `ban();`
   benutzen... Hier ist es richtig 😀
   ```php
   $player->setBanned($grund, /*True = Ja, False = nein*/true);
   ```
