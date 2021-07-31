# Universal Dynamic Input
[Supported Games](https://github.com/Venomalia/UniversalDynamicInput/blob/master/Games.md) | [Discord](https://discord.gg/vEQYMPxgSR) | [Changelog](https://github.com/Venomalia/UniversalDynamicInput/blob/main/Changelog.md) | [Dolphin forum](https://forums.dolphin-emu.org/Thread-universal-dynamic-input-texture-pack) | [DynamicInputTextureCreator](https://github.com/iwubcode/DolphinDynamicInputTextureCreator)

This is a custom button package that uses [**Dynamic Input Textures**](https://forums.dolphin-emu.org/Thread-introducing-dynamic-input-textures-a-new-feature-for-controller-icons) to create custom buttons in real time.
Unlike traditional custom button packs, you can change the contoler settings at any time and in any way you like
and since it is a function of dolphin, the actual intalation is very simple.
As the name suggests, I try to support as many games and input devices as possible and not to implement every game perfectly.

I am constantly expanding this project and i am open for suggestions

### [Download](https://github.com/Venomalia/UniversalDynamicInput/releases)

##  Installation:
**Windows**:
- you need Dolphin 5.0-13603 or [newer](https://de.dolphin-emu.org/download/).
- Place the **"DynamicInputTextures"** folder into Dolphin's **"load"** directory,
`"%UserName%\Documents\Dolphin Emulator\Load"`
or when in portebel mode (portable.txt),`Dolphin directory "\User\Load"`
- Open Dolphin, enter Graphics > Advanced tab > Check Load Custom Textures.
- If it does not work immediately, please check your Contoller settings.

As soon as you start a [supported game](https://github.com/Venomalia/UniversalDynamicInput/blob/master/Games.md), Dolphin should generate and load the textures.
Before **updating**, the old installation should be removed.

##  Screenshots:
![Image1](https://i.imgur.com/WIxE3IZ.jpg "Image1")
![Image2](https://i.imgur.com/3pcxh5P.jpg "Image2")

## Supported Inputs Devices:
- **DInput/0/Keyboard Mouse** - Keyboard and Mouse.
- **XInput/0/Gamepad** - XInput like Xbox360, Xbox One or Xbox Series X changeable to [DualShock](https://github.com/Venomalia/UniversalDynamicInput#DevicesTextureChanger).
- **Bluetooth/0/Wii Remote** - Connect Wii Remotes for Emulated Controllers.
- **DSUClient/0/BetterJoy** - Switch Pro controller, required [BetterJoy](https://github.com/Davidobot/BetterJoy).
- **DSUClient/1/BetterJoy** - Switch Joy-con, required [BetterJoy](https://github.com/Davidobot/BetterJoy).
- **DSUClient/0/DualShock4** - DualShock4 required [DS4windows](https://github.com/Jays2Kings/DS4Windows).
- **DInput/0/Bluetooth LE** - Xbox series x
- **DInput/0/Wireless Gamepad** - Switch Pro controller
- **DInput/0/Wireless Controller** - DualShock4
- **DInput/0/USB GamePad** - General DInput

### DevicesTextureChanger
With the **DevicesTextureChanger.bat** in **#DefaultDevices** you can exchange certain devices.

## Known Issues
- [InputSyntax]( https://wiki.dolphin-emu.org/index.php?title=Input_Syntax) are not supported, like **`button A`&`button B`**.
- Sticks, Dpad and motion controls are incomplete and currently difficult to implement with Dynamic Input Textures.
- Controls that are based on text cannot be changed, affected are
Mario Sunshine, Mario Kart Wii, F-Zero GX and Super Mario Galaxy1&2 and more.

## FAQ - Problem solving:
#### does it work with texture packs?
Yes, there are no known problems.

### does it work with netplay?
Yes, but there can be problems with wii games because only player 1 can use Wii Remote 1.

### The textures do not fit for my controller
try the [DevicesTextureChanger](https://github.com/Venomalia/UniversalDynamicInput#DevicesTextureChanger).

### do you accept game suggestions?
yes but i need the [texture dumps](https://forums.dolphin-emu.org/Thread-how-to-install-texture-packs-custom-textures-info) to implement it. dumps can send to me via [Discord](https://discord.gg/vEQYMPxgSR).

### Dolphin closes when I try to start my game.
probably the pack is faulty, report the pack with the controller used.

### I See ? Buttens,
This means that your controller is not recognised or the button cannot be assigned.
- [InputSyntax]( https://wiki.dolphin-emu.org/index.php?title=Input_Syntax) is not possible, only individual buttons are recognised.
- The contoler is not **port_1** for GC or **Wiimote_1** for Wii? Check Contoller settings.
- If you use BetterJoy, DS4Windows or any other DSUClient you have to name them correctly. Enter Controller Settings > alternative input sources
  Use the name "DualShock4" or "BetterJoy" for Switch controllers.
- You are using the wrong device or it is not supported? Check Supported Devices list.
  or you have several controllers? currently only the first one is supported!
  use **"XInput_0_Gamepad"** not **"XInput_1_Gamepad"**

### I do not see any changes,
- is the game [supported](https://github.com/Venomalia/UniversalDynamicInput/blob/master/Games.md)?
- Are custom textures active? Open Dolphin, enter Graphics > Advanced tab > Check **Load Custom Textures**.
- You are using the wrong device or it is not supported? Check [Supported Inputs Devices](https://github.com/Venomalia/UniversalDynamicInput#supported-inputs-devices).
- You use **Dolphin 5.0-13603** or newer?
- Is everything installed correctly? then a texture pack was generated for the game,
check Dolphin's `"load\Textures\"` directory a `#Generated_<GameName>` directory should be existing!
If it doesn't, you must have done something wrong.

### where can i ask questions?
you can use [Discord](https://discord.gg/vEQYMPxgSR) or [thread](https://forums.dolphin-emu.org/Thread-universal-dynamic-input-texture-pack) in dolphin forum.

## Credits:
### Special thanks:
[iwubcode](https://github.com/iwubcode) for this great feature.
and to all helpers for beta-tests, feedback, texture-dumps and other improvements.

Super Mario Galaxy [1](https://forums.dolphin-emu.org/Thread-super-mario-galaxy-1-hd-texture-mod)&[2](https://forums.dolphin-emu.org/Thread-super-mario-galaxy-2-hd-texture-mod) UI assets a created by **Razius**.

Phantasy Star Online 1&2UI assets a created by [LutheeMajestic](https://forums.dolphin-emu.org/Thread-phantasy-star-online-episode-i-ii-hd-ui-project).

I use waifu2x for some UI elements.

## License: CC BY 4.0
[![CC BY 4.0](https://i.creativecommons.org/l/by/4.0/88x31.png)](https://creativecommons.org/licenses/by/4.0/)