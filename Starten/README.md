# Starten

Hier der Code womit ihr das Plugin starten lassen
könnt. Natürlich müsst ihr auch eine plugin.yml
datei machen

```php
<?php

namespace tutorial; /*Die Über Ordner von der Main*/

```

Jetzt kommen die Imports. Die können je nachdem
was ihr machen wollt abweichen. Zum Starten
reichen die aber 😉

```php
use pocketmine\plugin\PluginBase;
use pocketmine\event\Listener;
use pocketmine\{
    Server,
    Player
};
```

Jetzt der Hauptteil 😀

```php
class Main/*Datei Name ohne .php*/ extends PluginBase implements Listener {
    public function onEnable(){
       $this->getLogger()->info("Plugin aktiviert");
       $this->getServer()->getPluginManager()->registerEvents($this, $this);
    }
}
```

Ganzer Code:
```php
<?php

namespace tutorial; /*Die Über Ordner von der Main*/

use pocketmine\plugin\PluginBase;
use pocketmine\event\Listener;
use pocketmine\{
    Server,
    Player
};

class Main/*Datei Name ohne .php*/ extends PluginBase implements Listener {
    public function onEnable(){
       $this->getLogger()->info("Plugin aktiviert");
       $this->getServer()->getPluginManager()->registerEvents($this, $this);
    }
}
```
