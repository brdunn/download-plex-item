<div align="center">

# Download Plex Item

[![License](https://img.shields.io/badge/license-Apache_2.0-red?style=for-the-badge&logo=none)](https://opensource.org/licenses/Apache-2.0)

Download Plex Item is a CLI tool that allows you to download items from a Plex Media Server to which you have access. You can either download a single item or download a tree of items.

</div>

## ⚡️ Quick Start
1. [Install Deno](https://docs.deno.com/runtime/getting_started/installation/). I recommend the `asdf` installation method. (A `.tools-version` file is included for convenience.)
1. Make the program executable. `chmod +x downloadPlexItem`

## ⚙️ Usage

### Example
 `./downloadPlexItem --serverUrl=https://1-2-3-4.56sdf234ssd2345.plex.direct:32400 --rootItemsRatingKeys=1456 --token=MY_X_PLEX_TOKEN --path="~/Downloads/"`

 ### Options

| Option | Description | Type | Default | Required? |
| --- | --- | --- | --- | --- |
| --serverUrl | The Url of the server from which you want to download the item. | `string` | | Yes |
| --rootItemsRatingKeys | A comma separate list of ratingKeys of the items you want to download. These can be the ratingKey of a show, season, or episode. | `string` | | Yes |
| --token | Your token for the previously specified server. | `string` | | Yes |
| --path | The destination to which to download the item. | `string` | `./` | No |

## ⚠️ Known Issues
- I've only tested this with movies and TV shows, seasons, and episodes. It may work to download music or photos, but your results may vary.
