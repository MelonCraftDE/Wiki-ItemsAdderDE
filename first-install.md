---
description: Wie man das Plugin installiert
---

# ⚙ Erste Installation

{% hint style="info" %}
Du solltest die erste Konfiguration auf einem Testserver auf deinem PC durchführen um Fehler und häufige Neustarts zu vermeiden. Spieler mögen es nicht wenn der Server offline ist.\
Du kannst die Daten zu deinem Hauptserver hochladen wenn du hier fertig bist.
{% endhint %}

{% hint style="danger" %}
Du solltest ALLE Installationsschritte befolgen, nicht nur den ersten.
{% endhint %}

## Schritt 1 - Installieren des Plugins und APIs

* Installiere [**ProtocolLib**](https://www.spigotmc.org/resources/protocollib.1997/)
* Installiere [**LoneLibs**](https://www.spigotmc.org/resources/lonelibs.75974/)
* (optional) Installiere **LightAPI** ([1.14, 1.15, 1.16](http://a.devs.beer/lightapi-old) | [1.17, 1.18](http://a.devs.beer/lightapi-new))
* (optional) Installiere [**Lib's Disguises**](https://www.spigotmc.org/resources/libs-disguises-free.81/) if you plan to create custom mobs in the future.
* Lege **ItemsAdder.jar** Datei in dein "plugins" Ordner
* Starte deinen Server
* Lass ItemsAdder **alles** fertig laden

Erster Schritt abgeschlossen.\
Jetzt geht es an **Schritt 2** um das **Ressourcenpaket** zu konfigurieren (keine Sorge, es ist nicht schwer) 
## Step 2 - resourcepack first installation

#### Entscheide dich für eine Hosting Methode:

{% content-ref url="plugin-usage/resourcepack-hosting/" %}
[resourcepack-hosting](plugin-usage/resourcepack-hosting/)
{% endcontent-ref %}

## Optionale Schritte

### Offiziellen ItemsAdder Inhalt hinzufügen

![](.gitbook/assets/items\_showcase\_gif.apng)

**ItemsAdder** kommt zusammen mit einer Menge Inhalten\
Sie sind nicht automatisch beim Download des Plugins dabei weil einige Spieler vielleicht nicht jedes Item oder Feature auf ihrem Server möchten.
#### Default pack

![](<.gitbook/assets/image (47).png>)

* Lade die aktuelle Version vom DefaultPack [hier](https://github.com/ItemsAdder/DefaultPack/releases/latest)&#x20;
* extrahiere den Inhalt in deinen **ItemAdder** Ordner und überschreibe alle Daten wenn du danach gefragt wirst
* führe dann den `/iazip` Befehl aus (und folge deiner [Hosting Methode](plugin-usage/resourcepack-hosting/) wenn du dich nicht für **self-host** entschieden hast).

#### Andere Packs (optional)

![](<.gitbook/assets/image (50).png>)

* Wenn du möchtest kannst du andere Packs Downloaden [hier](https://github.com/ItemsAdder/OtherPacks/releases/latest) which adds even more content
* extrahiere den Inhalt in deinen **ItemAdder** Ordner und überschreibe alle Daten wenn du danach gefragt wirst
* führe dann den `/iazip` Befehl aus (und folge deiner [Hosting Methode](plugin-usage/resourcepack-hosting/) wenn du dich nicht für **self-host** entschieden hast).

Wenn du auf Version 1.17 oder niedriger bist, musst du folgendes bei der Erzgenerierung ändern:

* Öffne diese Dateien und setze `enabled: true`.\
  `ItemsAdder\data\items_packs\iaalchemy\worlds_populators_old.yml`\
  `ItemsAdder\data\items_packs\iasurvival\ores\worlds_populators_old.yml`
* Öffne diese Dateien und setze `enabled: false`.\
  `ItemsAdder\data\items_packs\iaalchemy\worlds_populators_1_18.yml`\
  `ItemsAdder\data\items_packs\iasurvival\ores\worlds_populators_1_18.yml`

### Entfernen von Standard Items

{% content-ref url="faq/removing-default-stuff/" %}
[removing-default-stuff](faq/removing-default-stuff/)
{% endcontent-ref %}

### Vermeide glitched blocks

{% content-ref url="faq/blocks-minerals-issues/custom-blocks-glitch-texture/avoid-glitched-blocks.md" %}
[avoid-glitched-blocks.md](faq/blocks-minerals-issues/custom-blocks-glitch-texture/avoid-glitched-blocks.md)
{% endcontent-ref %}
