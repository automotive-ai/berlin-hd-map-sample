# Berlin HD map sample — JuniStraße

Public sample assets for a high-definition road network around **JuniStraße, Berlin** (Urban Road / `DE_UR` naming). The **OpenDRIVE map** is included now; **measurement drive data** and a matching **Unreal Engine** scene are optional follow-ups and are **not** in this repository yet.

## Repository layout

| Path | Contents |
|------|----------|
| [`maps/opendrive/`](maps/opendrive/) | OpenDRIVE (`.xodr`) road network for the scene |
| [`drive-data/`](drive-data/) | Reserved for measurement / drive recordings *(empty until you choose to publish)* |
| [`unreal-engine/`](unreal-engine/) | Unreal Engine project or export notes *(coming soon)* |
| [`docs/images/`](docs/images/) | Figures for this README (e.g. coverage / location map) |

## HD map

- **File:** [`maps/opendrive/DE_UR_Berlin_JuniStr_RR.xodr`](maps/opendrive/DE_UR_Berlin_JuniStr_RR.xodr)  
- **Format:** [ASAM OpenDRIVE](https://www.asam.net/standards/detail/opendrive/) — suitable for simulation, validation, and tooling that consumes lane-level road geometry.

## Drive data

There is **no** drive or sensor data in the repo at the moment. If you add it later, put it under **`drive-data/`** and follow the layout notes in [`drive-data/README.md`](drive-data/README.md).

## Unreal Engine scene

A 3D environment built from this map and data is **planned**. Status and any export/import notes will be tracked in [`unreal-engine/README.md`](unreal-engine/README.md).

## Preview image (optional)

To show the covered area on the GitHub repository page, add an image such as `docs/images/coverage.png` (map screenshot, satellite crop with outline, or similar), then uncomment the line below in this file:

<!-- Uncomment after adding the image:
![Coverage area — Berlin JuniStraße](docs/images/coverage.png)
-->

## License

If you redistribute the map or derived works, add a `LICENSE` file at the repository root that matches your rights to the data (e.g. your organization’s terms or a standard open license). Until then, assume **all rights reserved** unless you state otherwise in a license file.
