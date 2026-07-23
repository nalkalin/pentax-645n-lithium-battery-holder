# Pentax 645N / 645N II 锂电池仓

用于 Pentax 645N / 645N II 的 3D 打印锂电池改装电池仓。当前版本采用两节 3.7 V 锂电池串联（2S，标称 7.4 V、充满 8.4 V），配合 2S USB-C 充电/升压模块供电。

English documentation: [README.md](README.md)

![装配效果图](images/assembled-holder-perspective.png)

![六视图 contact sheet](images/six-view-contact-sheet.png)

![装入相机后的侧面实拍](images/installed-holder-side-view.jpg)

![装入相机后的底部实拍](images/installed-holder-bottom-view.jpg)

> 安全提醒：这是相机供电 DIY方案。两节电芯必须型号、容量、新旧程度和充放次数状态一致。装入前务必用万用表确认模块输出电压、正负极和是否短路。焊点及金属触点必须绝缘，不能让金属边缘接触、挤压或刺破电芯。请勿使用鼓包、破损或异常发热的电芯。

## 设计理念

Pentax 645N / 645N II 原装电池仓使用 6 节 AA 碱性电池。能凑合用，但对于经常拍摄的人来说并不理想：一次性电池消耗快、废弃电池多，也经常需要额外购买和携带备用电池。

项目目标：把原本依赖耗材的供电方式换成可重复充电的锂电方案，让中画幅胶片相机在今天依然更方便、更可持续地使用。两节锂电池串联并配合 2S 充电/升压模块，优势如下：

- 可重复充电，减少反复购买和丢弃一次性 AA 电池。
- 支持 USB-C 充电，可以用充电器、充电宝或外拍供电设备补电。
- 2S 电池组提供 7.4 V 标称电压，足够驱动相机。

## 适用型号

- Pentax 645N
- Pentax 645N II

## 仓库内容

| 路径 | 说明 |
| --- | --- |
| `models/` | 可直接打印的 STL 模型文件。 |
| `images/` | 装配参考图、剖面图和材料参考图。 |
| `docs/bill-of-materials.md` | 英文材料清单。 |
| `docs/printing-and-assembly.md` | 英文打印与装配说明。 |

## STL 文件

所有 STL 均为毫米单位，导入切片软件时请使用 100% 比例。

| 文件 | 近似尺寸 |
| --- | ---: |
| `models/pentax-645n-lithium-holder-body.stl` | 52.03 x 29.13 x 65.37 mm |
| `models/pentax-645n-lithium-holder-locking-base.stl` | 62.08 x 36.06 x 15.94 mm |
| `models/pentax-645n-lithium-holder-top-contact-retainer.stl` | 14.43 x 20.59 x 7.89 mm |
| `models/pentax-645n-lithium-holder-lower-contact-spacer.stl` | 12.09 x 24.78 x 5.48 mm |
| `models/pentax-645n-lithium-holder-bottom-contact-retainer.stl` | 15.02 x 21.20 x 3.69 mm |

## 推荐打印方式

- 推荐使用 SLA 树脂打印，尺寸精度更好，小螺丝孔、触点槽和卡扣细节更容易成型。
- 推荐层高：0.03-0.05 mm。
- 摆放方向：尽量避开关键接触面上支撑，避免形成封闭吸盘区域，打印后清理触点槽和螺丝孔。

## 材料清单

核心材料：

- 两个规格、容量和状态一致的 3.7 V 锂电池电芯，串联组成 2S 电池组。
- 适用于 2S 电池组的 USB-C 充电/升压模块；接线必须以所购模块的丝印和说明书为准。
- M2.5 x 6 mm 黄铜手拧螺丝。
- M2.5 黄铜六角螺母。
- M1.2 x 3 mm 黄铜一字槽小螺丝。
- 铜片、黄铜片或镍片，用于制作相机侧电池触点。
- 软硅胶线、热缩管、Kapton 胶带或其他绝缘材料。

![材料参考](images/hardware-screws-and-nuts.jpg)

![锂电池规格参考（实际需两节匹配电芯）](images/103450-lipo-cell.png)

![2S 锂电池充电/升压模块](images/2s-lithium-charge-boost-board.png)

## 装配流程

1. 以 100% 比例打印全部 STL 文件。
2. 清理外壳、触点槽、卡扣和螺丝孔。
3. 先空装主体、底座、M2.5/M1.2 螺丝和小固定件，确认配合顺畅。
4. 放入两节匹配的 3.7 V 锂电池，按 2S 串联方案接线；确认电芯没有被挤压、弯折或被尖锐边缘刮到。
5. 按模块说明书连接电池组、保护/充电端和输出端。
6. 用万用表确认电池组电压、模块输出电压、触点正负极和是否短路。
7. 对所有焊点和金属边缘做绝缘，再装入相机测试。

![装配剖面图](images/assembly-cross-section-detail.jpg)

## 开源许可

本项目使用 Creative Commons Attribution 4.0 International License 开源，详见 [LICENSE](LICENSE)。

Pentax 是 Ricoh Imaging Company, Ltd. 的商标。本项目为独立社区设计，与 Ricoh/Pentax 无隶属或官方背书关系。
