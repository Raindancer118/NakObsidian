# <font color = "orange">DBS - Lernen</font>
| **Relation**       | **Attribute(s)**                                    | **Primary Key (PK)** | **Foreign Key (FK)**                                         | **Zusatzinfo**                              |
|--------------------|----------------------------------------------------|-----------------------|----------------------------------------------------------------|---------------------------------------------|
| **Projekt**        | `ProNr`, `Name`                                    | `ProNr`               | –                                                              | –                                           |
| **Risikogruppe**   | `RGNr`, `Gruppe`                                   | `RGNr`                | –                                                              | –                                           |
| **Risiko**         | `RNr`, `Text`, `Prüfdatum`, `Auswirkung`, `Wkeit`, `RGNr` | `RNr`                 | `RGNr` → **Risikogruppe**(`RGNr`)                               | **1:N** (Risikogruppe → Risiko)            |
| **Maßnahme**       | `MNr`, `Verantwortlich`, `Titel`                   | `MNr`                 | –                                                              | –                                           |
| **Bedroht_durch**  | `ProNr`, `RNr`                                     | (`ProNr`, `RNr`)      | `ProNr` → **Projekt**(`ProNr`) <br> `RNr` → **Risiko**(`RNr`)   | **M:N** (Projekt ↔ Risiko)                 |
| **Fasst_zusammen** | `ProNr`, `RGNr`                                    | (`ProNr`, `RGNr`)     | `ProNr` → **Projekt**(`ProNr`) <br> `RGNr` → **Risikogruppe**(`RGNr`) | **M:N** (Projekt ↔ Risikogruppe)           |
| **Bearbeitet_durch** | `RNr`, `MNr`, `Prüfdatum`, `Status`              | (`RNr`, `MNr`)        | `RNr` → **Risiko**(`RNr`) <br> `MNr` → **Maßnahme**(`MNr`)      | **M:N** (Risiko ↔ Maßnahme) <br> + Beziehungsattribute |
