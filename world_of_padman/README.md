# World of Padman Egg

<div align="center">
  <img src="https://worldofpadman.net/wp-content/uploads/wop_header05.png" width="400px" alt="World of Padman Logo">
</div>

## Description
World of Padman (WoP) is an open-source first-person shooter game available for multiple platforms. It is based on the Quake 3 engine (ioquake3) and features a colorful, comic-style aesthetic with unique weapons and game modes.

## Configuration
| Variable | Description | Default |
| :--- | :--- | :--- |
| **Server Name** | The hostname displayed in the server browser. | `A World of Padman Server` |
| **RCON Password** | Password for remote administration. | `changeme` |
| **Game Version** | The version tag to download (e.g., `latest` or `1.7.0`). | `latest` |
| **Max RAM** | The amount of memory dedicated to the engine (`com_hunkMegs`). | `512` |
| **Server Visibility** | 1 = LAN, 2 = Internet (Master Server). | `2` |

## Ports
| Port | Protocol | Description |
| :--- | :--- | :--- |
| `27960` | UDP | Game Port (Default) |

## Docker Info
This egg uses the generic Debian image.
*   **Image:** `ghcr.io/pterodactyl/yolks:debian`

## Notes
*   **First Run:** The server may take a few moments to generate the `botfiles` and `AAS` (Area Awareness System) files on the first startup.
*   **Custom Maps:** Place custom `.pk3` files in the `wop` directory (or your configured `FS_GAME` folder).
