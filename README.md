# Open Opal

Howdy!
This is a very simple fork of [Open Opal] that tweaks some setting for better performance (way lower latency) and defaults that are more to my taste.
It uses (what I hope is) on-device downsampling of a 4K capture and outputs a 1080p stream. This should - I hope - result in a better image than what I think might just be quad binning of the 4K image in some other generic piece of meeting software.

### Recommended steps to run

* Install Unity Capture (will install an additional virtual camera)
* Install OBS (will install an additional virtual camera)
* Start the OBS virtual camera
* Run Open Opal

Open Opal should automatically (thanks to pyvirtualcam) pick the Unity Capture camera to stream to, which OBS can then manipulate and pass on to some other program.

### Installing dependencies

I recommend using pyenv with Python 3.8.10.

```bash
pip install -r requirements.txt
```

### Building

```
python setup.py distribute
```
### About

Fork of cansik's 2003 proof of concept. We are in no way associated with Opal Camera.
