<p align="center"><img src="web/static/image/icons/banner.png" alt="EveryNasa banner" title="EveryNasa"></p>

The program takes a picture from the NASA [website](https://apod.nasa.gov/apod) every day
and sets it as a background for your workspace.

### What EveryNasa can do?
- Installing wallpapers on your desktop
- Installing wallpapers on your desktop every day
- There is information about each photo
- You can add any photo to your favorites

### Contents
- [How to build](#how-to-build)
- [Solution or answers to possible problems](#solution-or-answers-to-possible-problems)
- [License](#license)

---

| Platform         	 | Status      	 | Latest version 	   | Get it on                                                                           	   |
|--------------------|---------------|--------------------|-----------------------------------------------------------------------------------------|
| Windows          	 | Available   	 | 2.3.1            	 | [.msi](https://github.com/Redume/EveryNasa/releases/download/v2.3.1/EveryNasa.msi)    	 |
| Linux            	 | Unsupported 	 | 1.6            	   | [Binary file](https://github.com/Redume/EveryNasa/releases/download/v1.6/EveryNasa) 	   |
| Android          	 | Available   	 | 1.7.1          	   | [Google Play](https://play.google.com/store/apps/details?id=ru.murzify.everynasa)   	   |
| MacOS            	 | Unavailable 	 | 	                  | 	                                                                                       |
| iOS              	 | Unavailable 	 | 	                  | 	                                                                                       |
| Wallpaper Engine 	 | Unsupported 	 | 1.0            	   | [Steam Workshop](https://steamcommunity.com/sharedfiles/filedetails/?id=2884180886) 	   |

---

### Solution or answers to possible problems
Any bugs / problems that are not covered by these questions, please open an [issue](https://github.com/Redume/EveryNasa/issues/new?assignees=&labels=bug&template=bug_report.md&title=Bug)

<details>
<summary>Windows</summary>
    <li>To make all functions work correctly, install the program anywhere except Program Files(x86) / Program Files</li>
</details>


<details>
<summary>Linux</summary>

- If you have a mistake with `ayatana-appindicator3-0.1`

    <details>
        <summary><b>Debian / Ubuntu / Mint</b></summary>
        <details>
            <summary><b>KDE Plasma</b></summary>

  ```shell
  $ sudo apt install gir1.2-appindicator3-0.1
  ```

  </details>
  <details>
  <summary><b>GNOME</b></summary>

    - Install the package
  ```shell
  $ sudo apt install gnome-shell-extension-appindicator
  ```
    - Open `Tweaks`
    - Go to `Extensions`
    - Enable `Kstatusnotifieritem/appindicator support`
</details>
</details>
</details>

### How to build
<details>
<summary></summary>

- Install [GoLang](https://golang.org/dl/). Recommended version: 1.19.1


- First make a build. If you want to create a build without a console window, then remove `-ldflags "-H windowsgui"` from the command

```shell
go build -ldflags "-s -H windowsgui"
```

- Create a build of the installation package

```shell
go-msi make -msi EveryNasa.msi --version <version> -s wix
```

- Done
</details>

---

### License
This project is licensed under the Apache-2.0 License - see the [LICENSE](LICENSE) file for details.

```
Copyright 2022-2023 Redume

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

### Third-party library licenses
- [getlantern/systray](https://github.com/getlantern/systray) — [Apache-2.0](https://github.com/getlantern/systray/blob/master/LICENSE)
- [gofiber/fiber](https://github.com/gofiber/fiber) — [MIT](https://github.com/gofiber/fiber/blob/master/LICENSE)
- [go-ole/go-ole](https://github.com/go-ole/go-ole) — [MIT](https://github.com/go-ole/go-ole/blob/master/LICENSE)
- [mattn/go-sqlite3](https://github.com/mattn/go-sqlite3) — [MIT](https://github.com/mattn/go-sqlite3/blob/master/LICENSE)
- [rodkranz/fetch](https://github.com/rodkranz/fetch) — [MIT](https://github.com/rodkranz/fetch/blob/master/LICENSE)
- [shirou/gopsutil](https://github.com/shirou/gopsutil) — [BSD-3](https://github.com/shirou/gopsutil/blob/master/LICENSE)
- [skratchdot/open-golang](https://github.com/skratchdot/open-golang) — [MIT](https://github.com/skratchdot/open-golang/blob/master/LICENSE)
- [twbs/bootstrap](https://github.com/twbs/bootstrap) — [MIT](https://github.com/twbs/bootstrap/blob/main/LICENSE)
- [LottieFiles/lottie-player](https://github.com/LottieFiles/lottie-player) — [MIT](https://github.com/LottieFiles/lottie-player/blob/master/LICENSE)
- [jquery/jquery](https://github.com/jquery/jquery) — [MIT](https://github.com/jquery/jquery/blob/main/LICENSE.txt)
