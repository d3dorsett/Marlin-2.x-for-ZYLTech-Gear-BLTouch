# Marlin-2.x-for-ZYLTech-Gear-BLTouch

configuration.h and configuration.adv for the ZYLTech Gear 3D printer. These can be used to overwright the default setting in Marlin v2.0.x, when creating a new Robin_nano35.bin using Microsoft Visio Code and PlatformIO  

Robin_nano35.bin for the ZYLTech Gear 3D printer. Copy the file to a SD card, insert into printer and power on. 

All changes and comments are tagged with // D3

*To switch from no probe, Freez ABL or BLTouch search for the following "Freez" or "BLTouch" in .h and .adv

*To switch from the default Marlin screen to the Nano screen search for the following "Nano menus" in both .h and .adv

configuration.h

// D3 21NOV2020 Disable ZYLTech Gear v2 MKS Robin Nano (Use M600 for Marlin menus. Use M25 for Nano menus.)

#define FILAMENT_RUNOUT_SCRIPT "M600"

// D3 07NOV2020 Enabled ZYLTech Gear v3 MKS Robin Nano (Enable for Marlin menus, Disable for Nano menus)

#define LCD_BED_LEVELING

// D3 21NOV2020 Disable ZYLTech Gear v2 MKS Robin Nano (Enable for Marlin menus, Disable and use TFT_LVGL_UI_FSMC for Nano menus)

#define FSMC_GRAPHICAL_TFT

// D3 21NOV2020 Disable ZYLTech Gear v2 MKS Robin Nano (Enalbe for Nano menus, Disable and use FSMC_GRAPHICAL_TFT for Marlin menus)

//#define TFT_LVGL_UI_FSMC  // Robin nano v1.2 uses FSMC

// D3 21NOV2020 Enabled ZYLTech Gear v2 MKS Robin Nano (Enable for Marlin menus, Disable Nano menus)

#define TOUCH_SCREEN

configuration.adv

// D3 21NOV2020 Enabled ZYLTech Gear v3 MKS Robin Nano (Enable for Marlin menus, Disable for Nano menus)

#define ADVANCED_PAUSE_FEATURE

Enjoy!

-D3
