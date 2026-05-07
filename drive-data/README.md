# Drive / measurement data

This folder holds **sensor and trajectory data** from mobile mapping drives that align with the HD map under [`../maps/opendrive/`](../maps/opendrive/).

## Berlin (current set)

- **Dataset:** Leica-style sensor package (trajectory CSV, camera JPEGs, LiDAR tiles as applicable).
- **`Tiles_<folderName>/`:** Contains **`chunks_index.json`** and the **LAS/LAZ tile subset** for this cut—the same layout that **Replimap** expects. Instead of the **original full LAS** from the survey; only compressed tiles intersecting this trajectory segment are kept.
- **Use:** Load the prepared folder in the RepliMap (**Load Sensor Data**) together with the matching OpenDRIVE map for Berlin.

HELLOO