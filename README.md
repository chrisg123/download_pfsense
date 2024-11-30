# Download pfsense

This script automates the process of downloading, verifying, and extracting the
**pfSense ISO file** from an official Netgate mirror.

## Features
- Downloads the pfSense ISO and checksum files from the official mirror.
- Validates the downloaded ISO file using its SHA256 checksum.
- Handles re-downloads if the file already exists or the checksum fails.
- Extracts the `.iso.gz` file to produce the final `.iso`.

## Usage
1. Clone this repository:
   ```bash
   git clone https://github.com/chrisg123/download_pfsense
   cd download_pfsense
   ```

2. Make the script executable:
   ```bash
   chmod +x dl_pfsense_iso
   ```

3. Run the script:
   ```bash
   ./dl_pfsense_iso
   ```

4. Follow the on-screen prompts if required.

## Requirements
- `bash`
- `curl`
- `sha256sum`
- `gunzip`

## Customization
You can modify the following variables in the script to customize its behavior:
- `DOWNLOAD_URL`: URL of the Netgate mirror.
- `PFSENSE_VERSION`: Desired pfSense version.

Download pfsense is released under the MIT License. See the [LICENSE](LICENSE)
file for more details.
