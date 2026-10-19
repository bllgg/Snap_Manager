# Snap Manager

A collection of lightweight bash utilities to free up disk space by removing redundant package manager data in Linux environments.

## Scripts

*   `clear_snap.sh`: Identifies and removes all disabled, older revisions of Snap packages currently stored by the `snapd` daemon.
*   `clear_pip.sh`: Purges the local Python `pip` cache (including built wheels and HTTP data) and reports the reclaimed storage.

## Usage

Ensure both scripts have execution permissions before running them:

```bash
chmod +x clear_snap.sh clear_pip.sh

# Run the pip cache cleanup
./clear_pip.sh

# Run the snap cleanup (requires elevated privileges)
sudo ./clear_snap.sh

