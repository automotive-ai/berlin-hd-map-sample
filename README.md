<p align="center">
  <img src="docs/images/aai_logo.png" alt="Berlin HD map sample — Str. des 17. Juni" width="420"/>
</p>

# Berlin HD map sample — Str. des 17. Juni

Public sample assets for a high-definition road network along **Str. des 17. Juni** in Berlin (Urban Road / `DE_UR` naming), covering the stretch from the **Brandenburg Gate** (*Brandenburger Tor*) to the **Victory Column** (*Siegessäule*). The repository includes the **measurement drive data**, a high-fidelity **OpenDRIVE map**, and a packaged **Unreal Engine** scene for visualization.

## Repository layout

| Path | Contents |
|------|----------|
| [`maps/opendrive/`](maps/opendrive/) | OpenDRIVE (`.xodr`) road network for the scene |
| [`drive-data/`](drive-data/) | Measurement / drive recordings (trajectory, camera, LiDAR) |
| [`unreal-engine/`](unreal-engine/) | Packaged Unreal Engine build for scene visualization |

## HD map

- **Coverage:** Str. des 17. Juni, Berlin — from the Brandenburg Gate to the Victory Column.  
- **File:** [`maps/opendrive/DE_UR_Berlin_StrDes17Juni_RR.xodr`](maps/opendrive/DE_UR_Berlin_StrDes17Juni_RR.xodr)  
- **Format:** [ASAM OpenDRIVE](https://www.asam.net/standards/detail/opendrive/) — suitable for simulation, validation, and tooling that consumes lane-level road geometry.  
- **Map details:** See [`maps/README.md`](maps/README.md) for geographic coverage, provenance, and a full list of what is modeled in the high-fidelity `.xodr`.

### Map preview

<p align="center">
  <img src="docs/images/MapPreview2.png" alt="OpenDRIVE map preview — Str. des 17. Juni, Berlin" width="920"/>
  <br/>
  <em>OpenDRIVE map loaded in <a href="https://www.automotive-ai.com/replimap">RepliMap</a>, overlaid on Mapbox satellite imagery.</em>
</p>

## Drive data

Leica-style sensor package (trajectory CSV, camera JPEGs, LiDAR tiles as applicable). The drive data shared in this repository is **loadable in [RepliMap](https://www.automotive-ai.com/replimap)** for editing, visualization, and enrichment alongside the HD map.

### RepliMap

[**RepliMap**](https://www.automotive-ai.com/replimap) is a unified platform designed for HD map editing and 3D scene editing for autonomous driving, enabling engineers to create, customize, and enrich road networks with precision.

## Unreal Engine scene

A 3D environment built from the **OpenDRIVE map** and **sensor / drive data** in this repository is available as a packaged **Unreal Engine** build for visualization. See [`unreal-engine/README.md`](unreal-engine/README.md) for how to run it.

For access beyond this visualization build (for example project source, integration, or commercial use), get in touch at **[sales@aai-innovations.com](mailto:sales@aai-innovations.com)**.

## License

Use of the map and any other materials in this repository is governed by **[`LICENSE`](LICENSE)** in the repository root: **no commercial use**, **no resale**, and **no reutilization** (e.g. incorporating the data into other products, services, or datasets) without written permission from the copyright holder(s). 
