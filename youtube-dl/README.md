## youtube-dl

Environment for running [youtube-dl](https://github.com/rg3/youtube-dl) in docker.

* built on top of `alpine` base image
* includes `ffmpeg` in order to allow `youtube-dl` stitch together high quality videos, which are generally served as separate audio and video tracks
* `youtube-dl` is the entrypoint of the image
* 124 MB

### Example usage:

Download a video:

```bash
$ docker run -it --rm -v /tmp:/tmp jbergknoff/youtube-dl -o /tmp/video.mp4 https://www.youtube.com/watch?v=ZWuNf4gxwuM
```