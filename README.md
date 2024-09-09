# Copa Chilena 2024 Stream Overlay

This overlay is intended to be used with [tosu](https://github.com/KotRikD/tosu). made by [shdewz](https://github.com/shdewz/4wc-stream-overlay) and [ilw8](https://github.com/ILW8)

## OBS Setup

Install fonts from `_shared/fonts` folder

### main scene  
| source        | url/path                                            | width | height | x         | y         |
|---------------|-----------------------------------------------------|-------|--------|-----------|-----------|
| vc_overlay*   |                                                     | 480   | 100    | 0         | 880       |
| osu clients** |                                                     | 480   | 360    | see below | see below |
| accents       | http://127.0.0.1:24050/cc24-stream-overlay/gameplay/| 1920  | 1080   | 0         | 0         |
| main_overlay  | http://127.0.0.1:24050/cc24-stream-overlay/main/    | 1920  | 1080   | 0         | 0         |

<sup>*url from discord, replace custom css with [vc.css](vc.css)</sup><br>
<sup>**normal 1v1 placement according to the following table:</sup>
| client | x    | y    |
|--------|------|------|
| 0      | 0    | 160  |
| 1      | 960  | 160  |


### mappool
| source           | url/path                                           | width | height | x | y   |
|------------------|----------------------------------------------------|-------|--------|---|-----|
| vc_overlay       |                                                    | 480   | 100    | 0 | 880 |
| mappool_overlay* | http://127.0.0.1:24050/cc24-stream-overlay/mappool/| 2220  | 1080   | 0 | 0   |
| main_overlay     | http://127.0.0.1:24050/cc24-stream-overlay/main/   | 1920  | 1080   | 0 | 0   |

### intro*
| source           | url/path                                         | width | height | x | y   |
|------------------|--------------------------------------------------|-------|--------|---|-----|
| intro_overlay    | http://127.0.0.1:24050/cc24-stream-overlay/intro/| 1920  | 1080   | 0 | 0   |

<sup>*data pulled from `_data/coming_up.json`, requires exchanging between matches</sup>

### winner
| source           | url/path                                          | width | height | x | y   |
|------------------|---------------------------------------------------|-------|--------|---|-----|
| winner_overlay   | http://127.0.0.1:24050/cc24-stream-overlay/winner/| 1920  | 1080   | 0 | 0   |

Intro and winner scenes can also have the vc overlay bottom left if needed

### Transitions



<sup>Fallback: add a **300ms `linear horizontal` luma wipe** transition between the scenes with **`0.05`** smoothness</sup>

### Interacting with the mappool
- Left click: left (red) team pick
- Right click: right (blue) team pick
- Ctrl+Click: ban
- Shift+Click: clear