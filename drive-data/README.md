# Drive / measurement data

This folder holds **sensor and trajectory data** from mobile mapping drives that align with the HD map under [`../maps/opendrive/`](../maps/opendrive/).

## Berlin (current set)

- **Dataset:** Leica-style sensor package (trajectory CSV, camera JPEGs, LiDAR tiles as applicable).
- **`Tiles_<folderName>/`:** Contains **`chunks_index.json`** and the **LAS/LAZ tile subset** for this cut—the same layout the Map Editor and **Replimap** expect. The **original full LAS** from the survey is **not** included here, to **save space**; only tiles intersecting this trajectory segment are kept.
- **Cut:** Trajectory and images are limited to **frame range 5878–6708** (1-based row indices in the full Sphere trajectory), i.e. a contiguous segment of the Berlin drive.
- **Use:** Load the prepared folder in the Map Editor (**Load Sensor Data**) together with the matching OpenDRIVE map for Berlin.