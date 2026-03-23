# Berlin HD map sample — JuniStraße

Public sample assets for a high-definition road network along **JuniStraße** in Berlin (Urban Road / `DE_UR` naming), covering the stretch from the **Brandenburg Gate** (*Brandenburger Tor*) to the **Victory Column** (*Siegessäule*). The **OpenDRIVE map** is included now; **measurement drive data** and a matching **Unreal Engine** scene are coming soon and are **not** in this repository yet.

## Repository layout

| Path | Contents |
|------|----------|
| [`maps/opendrive/`](maps/opendrive/) | OpenDRIVE (`.xodr`) road network for the scene |
| [`drive-data/`](drive-data/) | Reserved for measurement / drive recordings *(coming soon)* |
| [`unreal-engine/`](unreal-engine/) | Unreal Engine project or export notes *(coming soon)* |

## HD map

- **Coverage:** JuniStraße, Berlin — from the Brandenburg Gate to the Victory Column.  
- **File:** [`maps/opendrive/DE_UR_Berlin_JuniStr_RR.xodr`](maps/opendrive/DE_UR_Berlin_JuniStr_RR.xodr)  
- **Format:** [ASAM OpenDRIVE](https://www.asam.net/standards/detail/opendrive/) — suitable for simulation, validation, and tooling that consumes lane-level road geometry.

## Drive data

There is **no** drive or sensor data in the repo at the moment. Coming soon **`drive-data/`**.

## Unreal Engine scene

A 3D environment built from this map and data is **planned**. Status and any export/import notes will be tracked in [`unreal-engine/README.md`](unreal-engine/README.md).


<!-- Uncomment after adding the image:
![Coverage area — Berlin JuniStraße](docs/images/coverage.png)
-->

## License

Use of the map and any other materials in this repository is governed by **[`LICENSE`](LICENSE)** in the repository root: **no commercial use**, **no resale**, and **no reutilization** (e.g. incorporating the data into other products, services, or datasets) without written permission from the copyright holder(s). 
