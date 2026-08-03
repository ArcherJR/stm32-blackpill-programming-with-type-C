# stm32-blackpill-programming-with-type-C
I cant find enough source for stm32f401ceu6 dfu programming so I had to learn it on my own, and I prepared this repo so it would be useful to more people.

# 1 Gerekinimler / Requirements

- Stm32 blackpill development board
- data-enabled Type C cable
- arduino ide or vscode and platformio


# Type-C ile programlama / Programming with type-C 

*TR:* Stm32f401/411 blackpill kartlarında bulunan mcu lar dahili bootloader a sahiptir ve silinemez bu dahili bootloader sayesinde geliştirme kartımızı sadece bir type c kablou ile programlayacağız 

*EN:* The MCUs found on STM32F401/411 BlackPill boards feature an internal, non-erasable bootloader; thanks to this internal bootloader, we can program the development board using only a Type-C cable.

# Geliştirme kartını dfu moduna alma / Putting the development board into DFU mode 

*TR:* geliştirme kartını dfu moduna almak için kart üzerinde bulunan boot 0 butonuna yaklaşık 1 saniye basın ve elinizi çekmeden nrst butonuna bas çek yapın ardından boot0 ı bırakın. geliştirme kartı dfu moduna geçmiş olacak

*EN:* To put the development board into DFU mode, press and hold the BOOT0 button on the board for approximately one second; while holding it, press and release the NRST button, then release the BOOT0 button. The development board will then enter DFU mode.

# IDE konfigürasyonu / IDE configuration

*ARDUINO IDE*

file > prefences > Additional boards manager URLs > paste this: 

`
https://github.com/stm32duino/BoardManagerFiles/raw/main/package_stmicroelectronics_index.json
`

![Arduino settings](Arduino\ settings.png)
