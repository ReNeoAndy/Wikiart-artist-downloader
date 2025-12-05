# Wiki Art download by Artist


A simple Python script to download all paintings by a specific artist from [WikiArt.org](https://www.wikiart.org) along with structured metadata.

This script uses WikiArt's legacy JSON API endpoint to fetch artwork data and downloads the highest-available resolution images (by removing the `!Large.jpg` resize suffix).

[! NOTE] 
Currently tailored for a single artist but easily modifiable.

## Features

- Fetches all paintings for a given artist in one request
- Downloads highest-resolution images available
- Saves complete metadata as a clean JSON file
- Detailed logging to both console and `wikiart_log.txt`
- Generates a weird filename like look at it lol
- Skips already-downloaded images
- Graceful handling of interrupts (Ctrl+C)

## Requirements

- Python 
- `requests` library


Install the dependency with:

```bash
pip install requests
```

## A Quick Start (Single Artist)

1. Open the script `wikiart.ipynb`
2. Change the `artist_url` value (around line 76) to the desired artist:
3. run the script
