# CameraMotionDetection
Python class that detects camera motion and record a video.

**Prototype :**

`class MotionDetection (string path, int video_source, string video_size, float threshold, int time_interval, int recording_time, boolean show_camera, boolean show_mask, boolean debug)`

## Usage :

```python
# Instanciating the class
MD = MotionDetection("D:\\path\\record", 0, '1080p', 20000, 5, 1, True, False, False)

# Starting detection
MD.start()

# Stopping détection
MD.end()
```

## Attributes :

* `path` : Path of the directory to put the recorded files.
* `video_source` : Numeric value of the video source (in order to choose the right camera). Begin with 0.
* `video_size` : Resolution of the video ('4k', '1080p', '720p' ou '480p').
* `threshold` : Noise threshold of the motion detection (0 very sensible, 100000 not sensible).
* `time_interval` : Time interval in second between records.
* `recording_time` : Duration of the recording in second.
* `show_camera` : Boolean to show the camera view.
* `show_mask` : Boolean to show the motion mask.
* `debug` : Boolean to show the numeric values of the noise in the console.
