# Tauri Kaplay Template
[![Tauri logo](https://raw.githubusercontent.com/tauri-apps/tauri/dev/.github/splash.png)](https://tauri.app/)
[![KaPlay logo](https://github.com/marklovers/kaplay/raw/master/assets/brand/kaplay-o.webp)](https://kaplayjs.com/)

> (Click the image to go to each product's official website)
>
> `Tauri Kaplay Template` is not affiliated with Tauri or KaPlay

## Write once, deploy anywhere

The easiest way to build a game ever: Tauri + KaPlay.

Use the unlimited features powered by KaPlay to build your game in 30 seconds.

## Quick Start
Everything has been prepared for you.

To start editing, open `mygame/src/main.js`

The script is really easy to write, like this:

```javascript
import startGame from "kaplay"

const k = startGame()

k.loadSprite("bean", "sprites/bean.png")

k.add([
	k.pos(120, 80),
	k.sprite("bean"),
])

k.onClick(() => k.addKaboom(k.mousePos()))
```

## Testing
Testing is really easy, just run this command in the `mygame` folder:

```sh
npm run tauri dev
```

## Building
To build without any diffuculties, you need to type these commands:

```sh
sudo apt install libgtkd-3-dev
sudo apt install libsoup2.4-dev
sudo apt install libjavascriptcoregtk-4.0-dev
sudo apt install libwebkit2gtk-4.0-dev
```

> *P.S.* You can copy these above at once (including line feeds) and paste them at once in your terminal (for most terminal, you should use right click), the shell will automatically run each command.

And then you can build it by using:

```sh
npm run tauri build --verbose
```

Then, everything is done!

The binary file is at `mygame/src-tauri/target/release/bundle/appimage_deb/date/usr/bin/`!

The `.deb` package is at `mygame/src-tauri/target/release/bundle/deb/`!

> *P.S.* Due to unknown error, I can't build the appimage.
>
> The error message is like this:
>
> `Error failed to bundle project: error running appimage.sh`
>
> If anyone knows how to solve it, please tell me vis **Issue** or **Pull Request** or **My Email** (zzh__2020@outlook.com)
>
> Click [me](mailto:zzh__2020@outlook.com) to connect me by email!
>
> If sending email, please use `Tauri Kaplay Template Issue Solving!` as title, for there are too many academic rubbish in my inbox😂!