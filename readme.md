# Sample Keyboard Firmware
This is a keyboard firmware is for [aizuknight/sample_keyboard](https://github.com/aizuknight/sample_keyboard), and based on the [qmk\_firmware](https://github.com/qmk/qmk_firmware).

## Compile
```
qmk compile -kb sample_keyboard -km default
```

## Flash
```
qmk flash -kb sample_keyboard -km default
```
Push seeed xiao rp2040's RESET button while pushing its BOOT button.

## Additional Documentation
* [See the official documentation on docs.qmk.fm](https://docs.qmk.fm)
