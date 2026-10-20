Backrooms Entities (Fabric, Minecraft 1.21.1, GeckoLib 4)
Entities: Smiler, Hound, Skin-Stealer, Partygoer (je mit Spawn-Ei im Kreativmenue).
Bauen
JDK 21 installieren.
Projekt in IntelliJ IDEA oeffnen (Gradle-Import). Fehlt der Gradle-Wrapper:
`gradle wrapper --gradle-version 8.10.2` im Projektordner ausfuehren.
Versionen in `gradle.properties` mit https://fabricmc.net/develop abgleichen.
`./gradlew build` -> fertige Mod in `build/libs/backrooms-entities-0.1.0.jar`
Zum Testen: `./gradlew runClient`
Zum Spielen braucht ihr Fabric Loader, Fabric API und GeckoLib (1.21.1) im mods-Ordner.
Verhalten
Smiler: passiv, bis man ihn ansieht; verschwindet im Licht.
Hound: schnell, Rudel greift gemeinsam an.
Skin-Stealer: klaut mit 35 % Chance einen Hotbar-Gegenstand pro Treffer, droppt ihn beim Tod.
Partygoer: langsam, 60 HP, Gruppenangriff.
Anpassen
Spawn-Gewichte: `BackroomsMod.java` (BiomeModifications.addSpawn)
Werte/KI: `entity/*.java`
Modelle/Animationen: `src/main/resources/assets/backrooms/{geo,animations,textures}/entity/`
(Smiler = dein konvertiertes Modell; die anderen drei sind einfache Platzhalter zum Ueberarbeiten in Blockbench)
