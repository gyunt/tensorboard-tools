Tensorboard Tools (`tbtools`)
=============================

This is a random collection of utilities for inspecting TensorFlow summary files.

*Under development (so for personal use at this point)!*


## Image Viewer

Image summary in Tensorboard does suck. Run a server that would parse an event file:

```
python -m tbtools.image_viewer --event_file events.out.tfevents.1234567890
```

now we can inspect the images that are stored as image summary:

```
http://localhost:7006/<step>/<summary_tag>
http://localhost:7006/0/input_image/image/0
```


## TODO

- Advanced Image Viewer
- Draw matplotlib plots for scalar values (e.g. loss)
