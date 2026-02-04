# yumelinks 
a yume nikki style room and editor stored in a single html document

## uploading assets into html file dataurl embed:
all uploaded files must be under 20KiB
#### player spritesheet: 
- png, jpeg
- max size 512x512
- 4x4 animation sprites:
```
    foot in air
    |     feet on ground
    |     |     other foot in air
    v     v     v
 +1-----2-----3-----4----
1|up    up    up    blank
2|right right right blank
3|down  down  down  blank
4|left  left  left  blank
```
#### tileset
- png, jpeg
- max size 1024x1024
- 16x16 tile sheet
#### walk sound
- mp3, wav, ogg
- aim for less than a second long

#### TODO IMPLIMENT: alternatively you can add url to assets stored in folders or online

## putting it on your site
### if you place it within an iframe on your page and some functions do not work try adding these sandbox rules to the iframe
`sandbox="allow-scripts allow-popups allow-downloads""`
- `allow-scripts` is essential
- `allow-popups` is required for opening links on link tiles
- `allow-downloads` is required for saving from inside the iframe

### you can link to the page with x and y url parameters to start the player at a specific position
this is useful for if you want to have multiple doors leading into your dream
