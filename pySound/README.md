----- Driver
git clone https://github.com/waveshare/WM8960-Audio-HAT
cd WM8960-Audio-HAT
sudo ./install.sh
sudo reboot





## Requirements
+ [seeed-voicecard](https://github.com/respeaker/seeed-voicecard), the kernel driver for on-board WM8960 codec
+ [spidev](https://pypi.python.org/pypi/spidev) for on-board SPI interface APA102 LEDs
+ [google-assistant-library](https://github.com/googlesamples/assistant-sdk-python/tree/master/google-assistant-sdk/googlesamples/assistant/library)
+ [avs](https://github.com/respeaker/avs), Alexa Voice Service client python library
+ [voice-engine](https://github.com/voice-engine/voice-engine)

## Setup
1. Go to [seeed-voicecard](https://github.com/respeaker/seeed-voicecard) and install it
2. Use `raspi-config` to enable SPI.
3. Install `spidev` (`pip install spidev`).
4. Run `python pixels.py` to test the pixels.

## Build a Google Home like device with Google Assistant SDK
1. Setup [google-assistant-library](https://github.com/googlesamples/assistant-sdk-python/tree/master/google-assistant-sdk/googlesamples/assistant/library)
2. Run `python google_assistant.py --device_model_id 'respeaker-xyz'`

## Build an Echo like device with Alexa Voice Service
1. `pip install avs voice-engine`
2. Go to [snowboy](https://github.com/Kitt-AI/snowboy) and install its python binding.
3. `python alexa.py`
