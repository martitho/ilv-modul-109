# ilv-modul-109
Dieses Repositoy stellt eine Docker-Umgebung mit Authentisierung zur Verfügung.

## traefik
Dies ist der Reverse Proxy
traefik.ilv.local wird auf das Dashboard umgeleitet.

## authelia
Dies ist der Authentisierungsteil.
Benutzername und Passwort zum Testen sind:
authelia
authelia

Der Link: auth.ilv.ch
## service1
eine whoami Seite, die über authelia ein Login anfordert.
service1.ilv.local
## service2
Eine whoami Seite ohne Authentisierung.
service2.ilv.local

Diese vier DNS-Namen müssen in der hosts-Datei des aufrufenden Clients eingetragen werden:

    10.200.255.1		service1.ilv.local
    10.200.255.1		auth.ilv.local
    10.200.255.1		traefik.ilv.local
    10.200.255.1		service2.ilv.local

    Weitere Beschreibung folgt...
