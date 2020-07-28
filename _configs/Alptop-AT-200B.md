---
layout: config
title: Alptop AT-200B
---
- using homebridge-camera-ffmpeg
- authentication for rtsp disabled in camera config
- RaspberryPi seems to work with higher res but chokes

```json
{
	"platform": "Camera-ffmpeg",
	"cameras": [{
		"name": "Crib Camera",
		"videoConfig": {
			"source": "-re -i rtsp://192.168.88.198/channel1",
			"maxStreams": 2,
			"maxWidth": 1280,
			"maxHeight": 720,
			"maxFPS": 20
		}
	}]
}
```