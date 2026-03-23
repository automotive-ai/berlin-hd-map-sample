# Drive / measurement data

This folder is intentionally **empty** for now. When you publish **sensor and trajectory data** from drives that align with the HD map in [`../maps/opendrive/`](../maps/opendrive/), use the layout below.

## Suggested layout (when you add files)

Organize by session or date so filenames stay stable on GitHub:

```text
drive-data/
  README.md
  YYYY-MM-DD_session-name/
    metadata.json          # optional: vehicle, sensors, coordinate frame, map version
    ...                    # your logs, rosbags, CSV, etc.
```

## Large files

If recordings exceed GitHub’s file size limits, consider [Git LFS](https://git-lfs.github.com/) or hosting archives elsewhere and linking from this README.
