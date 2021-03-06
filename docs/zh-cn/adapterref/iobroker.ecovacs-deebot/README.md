---
translatedFrom: en
translatedWarning: 如果您想编辑此文档，请删除“translatedFrom”字段，否则此文档将再次自动翻译
editLink: https://github.com/ioBroker/ioBroker.docs/edit/master/docs/zh-cn/adapterref/iobroker.ecovacs-deebot/README.md
title: 适用于ioBroker的Ecovacs Deebot适配器
hash: T0ob73oJ4PwAa7s273V/xK0R8ip52IqyySOGm7/MLWo=
---
![标识](../../../en/adapterref/iobroker.ecovacs-deebot/admin/ecovacs-deebot.png)

![NPM版本](http://img.shields.io/npm/v/iobroker.ecovacs-deebot.svg)
![资料下载](https://img.shields.io/npm/dm/iobroker.ecovacs-deebot.svg)
![npm](https://img.shields.io/npm/dt/iobroker.ecovacs-deebot.svg)
![特拉维斯](https://travis-ci.org/mrbungle64/ioBroker.ecovacs-deebot.svg?branch=master)

＃适用于ioBroker的Ecovacs Deebot适配器
此适配器使用[ecovacs-deebot.js](https://github.com/mrbungle64/ecovacs-deebot.js)库。

＃＃ 楷模
###支持的型号
* Deebot 901
* Deebot OZMO 920
* Deebot OZMO 930
* Deebot OZMO 950

###这些模型可以正常工作
* Deebot苗条2
* Deebot N79系列
* Deebot 601
* Deebot 710/711（请参阅“已知问题”）
* Deebot 900
* Deebot U2
* Deebot OZMO 610
* Deebot OZMO 900
* Deebot OZMO T8系列

###这些模型应该可以工作
* Deebot M88
* Deebot 600/605
* Deebot OZMO T5
* Deebot OZMO苗条10
* Deebot U2 Pro /电源

＃＃ 安装
建议使用Node.js版本10或更高版本。

该适配器使用画布库，可能需要其他安装。
要获得全部功能，请安装以下软件包。

对于基于Debian的Linux系统，应执行以下命令：

```bash
sudo apt-get update
sudo apt-get install build-essential libcairo2-dev libpango1.0-dev libjpeg-dev libgif-dev librsvg2-dev
```

有关其他系统的说明，请访问https://www.npmjs.com/package/canvas#compiling

＃＃ 用法
*有关如何使用此适配器的信息可在[此处]（https://github.com/mrbungle64/ioBroker.ecovacs-deebot/wiki）中找到

＃＃＃ 状态
*有关状态的信息可以在[here]（https://github.com/mrbungle64/ioBroker.ecovacs-deebot/wiki/States-%28EN%29）（英文）和[here]（https://github.com/github .com / mrbungle64 / ioBroker.ecovacs-deebot / wiki / Datenpunkte-％28DE％29）（德语）

＃＃ 已知的问题
*对于Deebot Ozmo 930，建议每天安排一次[安排重新启动]（https://www.iobroker.net/#en/documentation/admin/instances.md#The%20page%20content）报告在大约30分钟后连接断开。 24小时
*某些清洁功能可能不适用于710/711。请暂时使用0.5.8版。
*“边缘”功能不适用于Deebot U2（而是启动自动清洁）

＃＃ 常问问题
*常见问题可以在[此处]找到（https://github.com/mrbungle64/ioBroker.ecovacs-deebot/wiki/FAQ）

##免责声明
我绝不隶属于ECOVACS。

## Changelog

### 1.1.0
* Stable release

### 1.0.13
* Using library version 0.5.6
* Some improvements and fixes

### 1.0.12
* Using library version 0.5.5
* Added some more T8 models
* Several improvements and fixes

### 1.0.11
* Enabled some features for OZMO 900
* Several minor improvements

### 1.0.10
* Using library version 0.5.4
* Several improvements and fixes
* Added available spot area boundaries to "map" channel (read only)

### 1.0.9
* Using library version 0.5.3
* Added some experimental features (for a few models only)
* Added option for virtual boundaries and some further improvements to adapter config
* Some improvements for js-controller 3.2.x

### 1.0.8
* Using library version 0.5.2 (0.5.2-beta.1)
* Added available virtualBoundaries channel for Deebot 900/901 and Ozmo 930 (read only)
* Added "volume" and buttons for resetting consumable values for 950 type models (920/950/T8)
* Improved synchronization of spot area buttons
* Add option for setting the language for spot area names
* Added some experimental features (for a few models only)
* Several enhancements and fixes
* Bump some dependencies

### 1.0.7
* Using library version 0.5.1 (0.5.1-beta.3)
* Initial support for Deebot U2 series
* Improved support for Ozmo T8 models
* (boriswerner) Fixed cleaning log for 950 type models (920/950/T8)
* (boriswerner) Added available virtualBoundaries to "map" channel (currently read only)
* Improved handling of device classes
* Several enhancements and fixes

### 1.0.6
* Using library version 0.5.0-beta.0
* Fix for running multiple devices
* Support for additional Ozmo T8 models
* Add option to synchronize spotArea buttons
* Set state value for triggered buttons to false
* Add option to suppress "unknown" value for "map.deebotPositionCurrentSpotAreaID" state
* Further enhancements and fixes

### 1.0.5
* Bump library to 0.4.25
* Initial support for Ozmo T8 and T8+
* Implement buttons for resetting consumable values (currently Deebot 900/901 and Ozmo 930 only)
* Several enhancements and fixes

### 1.0.4
* Bump library to 0.4.21
* Remove canvas from dependencies
* Several bugfixes and improvements (especially for N79 series)
* Possibility to specify the number of reruns for a spot area
* Spot areas in the "control" channel are now created automatically
* Remove number of spot areas from adapter settings
* Some refactoring
* Bump dependencies

### 1.0.1 - 1.0.3
* Added support for Ozmo T8 AIVI
* Compact mode support
* Added a button to save the last used custom area values
* Added buttons to rerun saved custom areas
* Some enhancements and fixes

### 1.0.0
* Stable release

### 0.0.1 - 0.6.5
* [Changelog archive](https://github.com/mrbungle64/ioBroker.ecovacs-deebot/wiki/Changelog-(archive)#059)

## License

MIT License

Copyright (c) 2020 Sascha Hölzel <mrb1232@posteo.de>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.