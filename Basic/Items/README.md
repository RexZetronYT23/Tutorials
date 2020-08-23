# Items
Um Items, oder das Spieler Inventar verwalten
zukönnen, braucht ihr diesen Import
```php
use pocketmine\item\Item;
```

# Item setzen
Items in einen bestimmten Slot setzen. 
```php
$player->getInventory()->setItem(0, Item::get(5, 0, 1));
```
Erklärung: 
`setItem(0, ...)` Die `0` ist der Slot. Die Hotbar,
hat die Slots `0`-`8`

`setItem(0, Item::get(5, 0, 1));` mit `Item::get()` gettet
man sich ein Item. In unserem Beispiel wäre das
ein Einchenholzbrett. Die `5` ist die ID. Die 
`0` das Meta, und die `1` die Anzahl.

# Items adden

Ein Item ins Inventar adden, ist eigentlich genauso
wie setzen. Aber beim adden wird das Item einfach
auf einen Slot gesetzt. Deswegen brauch man auch
keinen Slot angeben
```php
$player->getInventory()->addItem(Item::get(5, 0, 1));
```
