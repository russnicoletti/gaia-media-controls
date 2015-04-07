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
    <video src="about:blank" id="player"></video>
    <gaia-media-controls id="media-controls"></gaia-media-controls>
  </div>
```

## Example javascript 
```html
    var controls = document.getElementById('media-controls');
    var player = document.getElementById('player');

    controls.initialize(player);
    player.preload = 'metadata';
    player.onloadedmetadata = onLoadedMetadata;
    player.src = '...';

    function onLoadedMetadata() {
      player.play();
    }

    controls.addEventListener('play-button-click', function() {
      if (player.paused) {
        player.play();
      }
      else {
        player.pause();
      }
    }
```

