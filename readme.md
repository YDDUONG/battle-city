# 坦克大战复刻版（Battle City Remake）

在线版本地址 [http://shinima.pw/battle-city/](http://shinima.pw/battle-city/)

《坦克大战》是由日本南梦宫 Namco 游戏公司开发的一款平面射击游戏，于 1985 年发售。游戏以坦克战斗及保卫基地为主题，属于策略型联机类。

该 GitHub 仓库的版本是经典坦克大战的复刻版本，基于原版素材，使用 React 将各类素材封装为对应的组件。素材使用 SVG 进行渲染以展现游戏的像素风，可以先调整浏览器缩放再进行游戏，1080P 屏幕下使用 200% 缩放为最佳。此游戏使用网页前端技术进行开发，主要使用 React 进行页面展现，使用 Immutable.js 作为数据结构工具库，使用 redux 管理游戏状态，以及使用 redux-saga 处理复杂的游戏逻辑。

目前游戏仍在开发中，只支持单人游戏，AI 设置不太合理，[欢迎体验](http://shinima.pw/battle-city/)。我的目标是实现完整的坦克大战复刻版，但仍有许多部分还未完成，希望在 2018 暑假结束（研二结束）之前完成。

与原版游戏不同，此版本中提供了关卡选择功能，玩家可以直接选择某个关卡开始游戏（因为我知道你没那么多时间一关一关玩下去 (●ˇ∀ˇ●)）。该版本提供了一个新颖的 [地图编辑器](http://shinima.pw/battle-city/#/list) 用于创建自定义游戏，相比经典版本会方便不少。你也可以在 [gallery 页面](http://shinima.pw/battle-city/#/gallery) 中浏览所有的组件，更好地了解游戏中各个的元素。

在 _[docs（施工中）](/docs)_ 文件夹中放了一些我在设计开发该游戏时的思考，对这个游戏感兴趣的同学可以看看。

<!-- TODO 坦克大战 文章链接 -->

### 开发进度：

**Milestone 0.2** （2018 年 4 月 15 日）

* [x] 游戏的基本框架
* [x] 给游戏中各个元素设置正确的生命周期
* [x] 从自定义的关卡中直接开始游戏
* [x] Gallery 页面重构
* [ ] 已知 BUG 修复

**Milestone 1.0** （2018 年 8 月 31 日）

* [ ] 更智能更合理的电脑玩家
* [x] 渲染性能优化
* [ ] 完整的游戏音效
* [ ] 双人模式
* [ ] 完整的设计、开发文档

### 本地开发版本

1.  克隆该项目到本地目录
2.  运行 `yarn install` 来安装依赖 （或者使用 `npm install`）
3.  运行 `yarn start` 开启 webpack-dev-server，并在浏览器中打开 `localhost:8080`
4.  运行 `yarn build` 来打包生产版本，打包输出在 `build/` 文件夹下

`devConfig.js` 包含了一些开发用的配置项，注意修改该文件中的配置之后需要重启 webpack-dev-server
