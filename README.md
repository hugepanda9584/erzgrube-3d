# Erzgrube 3D

Ein browserbasiertes 3D-Bergbauspiel mit lokaler Weltberechnung und Multiplayer über WebRTC.

## Spielen

Öffne die [Spielseite](https://hugepanda9584.github.io/erzgrube-3d/). Für Multiplayer öffnen alle dieselbe Seite. Ein Spieler wählt **Mit Freunden spielen → Neue Welt hosten** und teilt den Raumcode. Freunde tragen ihren eigenen Namen und den Code ein und wählen **Beitreten**.

Spielerpositionen und abgebaute Blöcke werden zwischen den Browsern ausgetauscht. Der Host verwaltet die gemeinsame Welt und muss während der Runde online bleiben; Weltänderungen werden auf seinem Gerät gespeichert. PeerJS Cloud vermittelt den Verbindungsaufbau. Manche Netzwerke benötigen zusätzlich ein TURN-Relay.

## Veröffentlichung

`index.html` ist die veröffentlichte Spielversion. Der Workflow in `.github/workflows/pages.yml` veröffentlicht Änderungen automatisch mit GitHub Pages.
