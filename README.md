![R3E](https://cloud.githubusercontent.com/assets/12783101/8024034/cd3c7c84-0d24-11e5-9e5f-3bf6fbab713f.png)

---

![Preview](https://raw.githubusercontent.com/sector3studios/webhud/master/src/img/preview.jpg)

# Web Hud

This is a sample showing how to create a web hud using the shared memory API for
[RaceRoom Racing Experience][r3e] (R3E).

For discussions or support go [here](https://forum.sector3studios.com/index.php?threads/in-gameplay-web-overlays.12947/).

## Quick start 快速开始

-   当前工程在线访问在游戏中有点问题,不会显示.可以使用官方服务https://github.com/sector3studios/webhud
-   如果要使用汉化版工程需要下载r3e_hud.7z,并解压.下载地址`https://share.weiyun.com/5j8MiuZ`
-   然后运行里面的serverstart.bat,会检测是否已经安装node.js环境,如果没有会自动安装node.js,连续下一步安装完成即可,或者直接安装里面的node-v12.14.0-x64.msi.再次运行serverstart.bat
-   解压 [public/dash.zip](public/dash.zip)
-   解压后运行里面的dash.exe
-   在Steam中右键属性->设置启动选项->将参数`-webdev -webHudUrl=http://localhost:4000/`加入进去保存
-   启动游戏

## Development

-   Development requires node/npm
-   For this to work you need to be running `public/dash.zip/dash.exe`. It is the source of all the data being used.
-   Run `npm install` to install all dependencies
-   Start development by running `npm start` and opening http://localhost:4000/
-   Add `-webdev -webHudUrl=http://localhost:4000/` to the game launch arguments
-   When you are happy with your changes run `npm run build` and the final files will be put in the `dist/` folder.

## Tips

-   Look at `src/types/r3eTypes.ts` to see what data is exposed
-   Press `Shift+i` to view the current game state (search takes regex)
-   Press `Shift+Space` to freeze the current game state
-   Press `Shift+d` to dump current game state as JSON into clipboard
-   Press `Ctrl+v` to insert dumped JSON game state into current session

## License

See [LICENSE](LICENSE).

[r3e]: http://game.raceroom.com/
