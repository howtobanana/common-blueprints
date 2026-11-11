# Common Blueprints

Home Assistant Blueprint-Suite für geräteunabhängige Automationen (Klima, Komfort, Verbrauch).
Im Gegensatz zu den Hersteller-Suites (Vaillant, Ökofen) sind diese Blueprints **generisch** und arbeiten mit beliebigen Entities (Switches, Sensoren).

## Module

| Modul | Status | Beschreibung |
|---|---|---|
| Geofencing | ✅ Läuft (Wien) | Abwesend-Helfer aus Entfernung und Personen, Vorheizen beim Heimweg (aus/automatisch/mit Bestätigung). Herstellerunabhängig – die Heizungssteuerung (z. B. Heating Core) liest nur die Helfer. Hervorgegangen aus „(Vaillant) Geofencing“ |
| Lüftungs-Steuerung | ✅ Läuft (Wien) | Lüft-Erinnerung (Zeit, CO2, Feuchte), Fenster-Timer und Eskalation, Regen/Sturm/Abwesend-Warnung, Sommer-Kühlung, mobile Klimaanlage. Hervorgegangen aus „(Vaillant) Lüftungs-Steuerung“ |
| Luftentfeuchter-Steuerung | 🚧 In Arbeit | Schaltet Luftentfeuchter im günstigen Stromfenster bei hoher Feuchtigkeit, mit Hysterese und Mindestlaufzeit |

## Installation
In HA unter `config/blueprints/automation/common/` ablegen (Wien: so eingerichtet). Push-Aktionen heißen `GEOFENCING_PRE_HEAT_CONFIRM`, `LUEFTUNG_SNOOZE_1H`, `LUEFTUNG_MUTE_UNTIL_CLOSED`, `LUEFTUNG_AC_WEITERLAUFEN`, `LUEFTUNG_AC_JETZT_AUS`.

## Autor
Fabian Brandl
