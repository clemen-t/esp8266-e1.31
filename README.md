# Controleur Pixel Wifi

## Objectif du projet
- Développement d'un controleur wifi basé sur un ESP8266
- Code open source
- Up to 4 universes
- Développement d'un PCB

## Hardware
  - ESP8266
  - LEDs pixels (WS2811 / WS2812)
  
### Montage :
  ![Texte alternatif](http://zupimages.net/up/17/17/pits.jpg)
  
## Avancement
- Fonctionne avec 1 universe (24/04/17)

## Programmation
* Programmer un ESP8266 avec l'IDE Arduino
  - installer l'IDE Arduino
  - Aller dans `fichier > préférences`, Dans la case "Additional Boards Manager URLs", entrez l'adresse suivante
    ```
    http://arduino.esp8266.com/staging/package_esp8266com_index.json
    ```
    ![Texte alternatif](https://image.noelshack.com/fichiers/2017/17/1493056662-capture-arduino.png)
    
  - Puis, aller dans `outils > Type de carte > Boards manager`, rechercher `esp8266`
    ![Texte alternatif](https://image.noelshack.com/fichiers/2017/17/1493056662-sans-titre.png)
  - Cliquer sur "install"
    ![Texte alternatif](https://image.noelshack.com/fichiers/2017/17/1493056662-capture-board.png)
  - Dans `outils > type de carte`, Vous devriez voir apparaitre une nouvelle option `Generic ESP8266 Module`
* Flasher le code dans l'ESP8266 (Cette partie sera mise à jour lorsque notre propre code sera fonctionnel)
  -  Telecharger le code disponible sur ce dépot : https://github.com/forkineye/E131
  -  Ouvrer l'exemple `ESP8266_NeoPixel` avec l'IDE Arduino
  -  Modifier les lignes suivantes :
        ```
        #define NUM_PIXELS 150  /* Nombre de LEDs */
        #define UNIVERSE 1      /* Universe */
        #define CHANNEL_START 1 /* Channel de départ */
        #define DATA_PIN 5      /* Sortie GPIO5 */

        const char ssid[] = "........";         /* SSID de votre box */
        const char passphrase[] = "........";   /* mot de passe de la box */
        ```
  -  Ouvrir le terminal Arduino et le serveur DHCP attribu une adresse IP, celle ci est affiché sur le terminal

* Xlights (Ce tuto n'a pas but de développer en détail le logiciel xLights)
  - Dans le menu `setup`, cliquer sur `ADD E1.31` et parametrer celui ci avec l'adresse IP obtenu sur l'ESP8266
  ![Texte alternatif](https://image.noelshack.com/fichiers/2017/17/1493056661-capture.png )

### Todos
  + Software
    - 4 Universes
  + Hardware
    - PCB

### lien
- https://www.fais-le-toi-meme.fr/fr/electronique/tutoriel/programmes-arduino-executes-sur-esp8266-arduino-ide
