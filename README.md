## Custom MIDI output device patch for 東方永夜抄　～ Imperishable Night

### Installing

1. Copy the `protosphere` directory to the root of wherever thcrap is installed.
2. Add `protosphere/custom_midi_output/` to your patch configuration, e.g.:
   
    ```
    {
      "console": false,
      "dat_dump": false,
      "patches": [
          {
            "archive": "protosphere/custom_midi_output/"
          },
          {
            "archive": "thpatch/lang_en/"
          }
      ]
    }
    ```

3. Change the value of "code" in `protosphere/custom_midi_output/global.js` to your desired output device ID (in hex notation). For example:

    ```
    "code": "01"
    ```

    Will use the MIDI device with an ID of 1 for output.