# CitizenQuack — open source sensor ducks

> "Design ducks not boxes. Make sensors make sense."

Started 2026-11-24.

## Concept (from references)

Environmental sensor nodes housed in 3D-printed ducks, so the data has a face.
Instead of a black box reading "PM2.5 = 38", a duck that has "gone a bit orange"
(posture, colour, sound) tells people what is going on. Each duck is a **fork**:
same sensor internals, a different shell and personality, co-designed with the community.

Versions so far:

| | Fab25 version (Jul 2025) | CitizenQuack SG (Sep 2026) | Maker Faire Shenzhen 2026 (in progress) |
|---|---|---|---|
| Focus | **Water** quality, floating river nodes | **Air** quality (PM2.5), humidity, noise | TBD: water, air or both |
| Electronics | Seeed SenseCAP K1100 (LoRa + AI kit) | Smart Citizen Kit #18929 (Geylang East) | TBD |
| Network | LoRa / Meshtastic | Smart Citizen → PLANETAI node (unofficial) | TBD |
| Parameters | temp, pH, turbidity, DO, EC/TDS (planned) | PM2.5 (+ humidity, noise possible) | TBD |
| Enclosure | 3D-printed duck, TPU ideal; weighted keel; probes on underside; pulsing LED eye | 3D-printed duck shell, forkable species; origami hat; pond float tests on fishing line | Starting from Miriam's Duck Options (`cad/miriam-duck-options/`); materials TBD |
| License | CC BY | — (not stated) | CC BY 4.0 |

### Fab25 design notes
- Matte white (contemporary) or bright yellow (visibility); recycled/recyclable, modular for repair.
- Weighted keel for floating stability; probes integrated on the underside, protected from debris.
- Gently pulsing LED in the eye = transmitting.
- Build listed: SenseCAP K1100, Meshtastic, hot glue gun. Status: work in progress (~8 h).

### Maker Faire Shenzhen 2026 version
In progress. Open decisions:
- [ ] Water or air (or both)?
- [ ] Electronics: SenseCAP K1100 / XIAO + Meshtastic / Smart Citizen Kit?
- [ ] What does the duck *do* with the data (LED colour, posture, sound, textile change)?
- [ ] Shell materials: soft / textile / biomaterial elements?
- [x] License: CC BY 4.0 (matches the Fab25 version).
- [ ] OSH documentation: BOM, assembly guide.

## Team / lineage

### Core contributors
- [YeEun "Miriam" Choi](https://fabacademy.org/2019/labs/seoul/students/miriam-choi/mev2.html) — main designer
- [Saad Chinoy](https://www.hackster.io/saad-chinoy)
- [Óscar González](https://www.linkedin.com/in/oscgonfer/)
- [Adai Suri](https://fablabbcn.org/team/adai-suri)
- [Claire Chaikin-Bryan](https://www.linkedin.com/in/claire-chaikin-bryan/)
- [Alberto Blanco](https://class.textile-academy.org/2026/jose-blanco/project/)

### Lineage
- Fab25 team: Saad Chinoy, Óscar González, Adai, Miriam Choi.
- SG page team: Saad Chinoy, YeEun "Miriam" Choi, Alberto Blanco, Jinger Zeng,
  Claire Chaikin-Bryan, Selena Pere, Robert Bogs; support from Violet Su (Seeed Studio).
- Origin: met at FAB24 Mexico; came together at FAB25 Czechia during Fab Lab Barcelona's
  "Smart Citizen Meets Meshtastic" hackathon (SCK 3.0 + LoRa/Meshtastic).

## Resources
- Fab25 version (Hackster page): https://www.hackster.io/citizenquack/citizenquack-lora-water-sensors-made-relatable-b8ba4e
- CitizenQuack SG post: https://ediblemakerspace.com/citizenquack-sg/
- Live feed page: https://ediblemakerspace.com/citizenquack
- PLANETAI (Fab City Foundation): https://planetai.fab.city/
- 3D files:
  - Duck body v4 STL: https://ediblemakerspace.com/wp-content/uploads/2026/11/duckbodyv4.stl_.zip
  - Duck options — head, body, 2 mm hollow (Miriam Choi): https://ediblemakerspace.com/wp-content/uploads/2026/11/27006BC0-DB1C-4D09-A989-8DFCE3DF78B9-DuckOptions.zip → downloaded to `cad/miriam-duck-options/`

## Folder layout
```
CitizenQuack/
  README.md        this file
  cad/             duck shells, keel, sensor mounts
  electronics/     wiring, BOM
  firmware/        code
  docs/            process photos, documentation
```

## License

This project is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/) — see [LICENSE](LICENSE).
You may share and adapt it for any purpose, as long as you give appropriate credit.
