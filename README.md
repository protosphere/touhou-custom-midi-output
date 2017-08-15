## Custom MIDI output device patch for Touhou Windows games

### Supported Versions

* 東方妖々夢　～ Perfect Cherry Blossom:
    * v1.0.0b

* 東方永夜抄　～ Imperishable Night:
    * v1.0.0b
    * v1.0.0c
    * v1.0.0d

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
          },
          ...
      ]
    }
    ```

3. Change the value of "code" in `protosphere/custom_midi_output/global.js` to your desired output device ID (in hex notation). For example:

    ```
    "code": "01"
    ```

    Will use the MIDI device with an ID of 1 for output.