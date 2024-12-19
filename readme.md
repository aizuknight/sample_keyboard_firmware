# Sample Keyboard Firmware
This is a keyboard firmware is for [aizuknight/sample_keyboard](https://github.com/aizuknight/sample_keyboard), and based on the [qmk_firmware](https://github.com/qmk/qmk_firmware).

## Prepare Your Build Environment
- For Windows, follow the instruction [here](guides/windows.md).
- For macOS, follow the instruction [here](guides/macos.md)
- For Linux/WSL, follow the instruction [here](guides/linux_wsl.md)
- For FreeBSD, follow the instruction [here](guides/freebsd.md)

## Clone This Repository
Next, execute the following command in your terminal(QMK MSYS for Windows).
```
cd /your/favorite/directory/
git clone --recursive https://github.com/aizuknight/sample_keyboard_firmware.git
cd sample_keyboard_firmware
qmk setup -y
```

## Compile
To compile sample_keyboard's firmware, execute the following command in your terminal(QMK MSYS for Windows).
```
qmk compile -kb sample_keyboard -km default
```

## Flash
To flash sample_keyboard's firmware into the microcontroller, execute the following command in your terminal(QMK MSYS for Windows).
```
qmk flash -kb sample_keyboard -km default
```
Connect the keyboard to your PC while holding down the BOOT button, or while connected to the PC, hold down the BOOT button and press the RESET button. After that, qmk will automatically flash into it.

## Additional Documentation
* [See the official documentation on docs.qmk.fm](https://docs.qmk.fm)
