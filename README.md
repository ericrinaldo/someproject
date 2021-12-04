

## förutsättning
- ha php 8 i datorn (`php -v`)
- ha composer (`composer -v`)
- öppna terminalen, navigera till denna mapp


## steg (demo)
1. installera paket: `composer install`
2. titta på innehållet i 'src/someFile.php'
3. kör rector utan att spara: `vendor/bin/rector process --dry-run`
  - (se potentiella ändringar i terminalen)
4. kör rector och spara: `vendor/bin/rector process`
5. titta på innehållet i **src/someFile.php** och se att det ändrats


## notera 
- målfiler, de som behandlas, satt i **rector.php:15**
- målversion satt i **rector.php:18**


## vad jag gjorde
- skapade en ny mapp ('someProject') och gick in i den
- initierade ett pojekt: `composer init`
- lade till paketet rector: `composer require rector/rector --dev`
- initierade rector konfiguration `vendor/bin/rector init`
- uppdaterade rector konfigurationen, för att sätta målversion



## källor
- https://getrector.org/blog/2020/11/30/smooth-upgrade-to-php-8-in-diffs
 https://github.com/rectorphp/rector
- https://getrector.org/blog/how-to-bump-minimal-version-without-leaving-anyone-behind

