## Overview
Playback controls for audio or video elements

## Installation

```bash
$ bower install gaia-components/gaia-media-controls
```

## Demo

- [demo](http://russnicoletti.github.io/media-controls/)

## Example html
```html
  <div id="player-container">
    <video src="about:blank" id="player" autoplay="true"></video>
    <gaia-media-controls id="media-controls"></gaia-media-controls>
  </div>
```

## Example javascript 
```html
    var controls = document.getElementById('media-controls');
    var player = document.getElementById('player');

    controls.attachTo(player);
    player.preload = 'metadata';
    player.src = "http://videos-cdn.mozilla.net/serv/webmademovies/Moz_Doc_0329_GetInvolved_ST.webm";
```

