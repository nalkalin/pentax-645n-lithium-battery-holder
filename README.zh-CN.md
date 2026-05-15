# Pentax 645N / 645N II 锂电池仓

这是一个用于 Pentax 645N / Pentax 645N II 的 3D 打印锂电池改装电池仓。模型按 103450 规格 3.7 V 聚合物锂电池和小型锂电充放/升压模块设计。

English documentation: [README.md](README.md)

![装配效果图](images/assembled-holder-perspective.png)

![六视图 contact sheet](images/six-view-contact-sheet.png)

> 安全提醒：这是相机供电 DIY 改装。装入相机前，请一定用万用表确认升压板输出电压和最终触点正负极。焊点和金属触点必须绝缘，不能让金属边缘接触或挤压锂电池软包。不要使用鼓包、破损或异常发热的锂电池。

## 设计理念

Pentax 645N / 645N II 原装电池仓使用 6 节 AA 碱性电池。这个方案当然能用，但对于经常拍摄的人来说并不理想：一次性碱性电池消耗快、废弃电池多，也经常需要额外购买和携带备用电池。

这个项目的目标不是为了改而改，而是把原本依赖耗材的供电方式换成可重复充电的锂电方案，让这些中画幅胶片相机在今天依然更方便、更可持续地使用。使用聚合物锂电池配合充放/升压模块，有几个明显好处：

- 可重复充电，减少反复购买和丢弃一次性 AA 碱性电池。
- 支持 USB-C 充电，可以用充电器、充电宝或外拍供电设备补电。
- 外出拍摄时不用携带和更换多节散装电池。
- 内部供电结构更紧凑，用一块软包电芯和稳压输出模块完成供电。

锂电池本身也需要正确使用、保护和回收。本设计的理念是减少一次性电池消耗，同时保留对电池安全的尊重。

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
| `models/pentax-645n-lithium-holder-body.stl` | 52.03 x 30.33 x 64.87 mm |
| `models/pentax-645n-lithium-holder-locking-base.stl` | 61.59 x 36.36 x 16.00 mm |
| `models/pentax-645n-lithium-holder-top-contact-retainer.stl` | 14.43 x 20.59 x 7.89 mm |
| `models/pentax-645n-lithium-holder-lower-contact-spacer.stl` | 12.09 x 24.78 x 5.48 mm |
| `models/pentax-645n-lithium-holder-bottom-contact-retainer.stl` | 15.02 x 21.20 x 3.69 mm |

## 推荐打印方式

- 推荐使用 SLA/MSLA/DLP 树脂打印，尺寸精度更好，小螺丝孔、触点槽和卡扣细节更容易成型。
- 推荐树脂：韧性树脂、类 ABS 树脂，或其他抗冲击能力较好的工程树脂。
- 推荐层高：0.03-0.05 mm。
- 摆放方向：尽量避开关键接触面上支撑，避免形成封闭吸盘区域，打印后清理触点槽和螺丝孔。

## 材料清单

核心材料：

- 103450 规格 3.7 V 聚合物锂电池，参考容量约 2000 mAh。
- USB-C 锂电充放/升压模块，参考图片上的焊盘为 `B+`、`B-`、`VO+`、`VO-`。
- M2.5 x 6 mm 黄铜手拧螺丝。
- M2.5 黄铜六角螺母。
- M1.2 x 3 mm 黄铜一字槽小螺丝。
- 铜片、黄铜片或镍片，用于制作相机侧电池触点。
- 软硅胶线、热缩管、Kapton 胶带或其他绝缘材料。

![材料参考](images/hardware-screws-and-nuts.jpg)

![103450 锂电池](images/103450-lipo-cell.png)

![锂电充放/升压模块](images/lithium-charge-boost-board.jpg)

## 装配流程

1. 以 100% 比例打印全部 STL 文件。
2. 清理外壳、触点槽、卡扣和螺丝孔。
3. 先空装主体、底座、M2.5/M1.2 螺丝和小固定件，确认配合顺畅。
4. 按相机电池仓触点位置裁切并弯折铜片/黄铜片/镍片。
5. 放入 103450 锂电池，确认没有挤压、弯折或被尖锐边缘刮到。
6. 固定锂电充放/升压模块，并安排好 USB-C 口和走线位置。
7. 将电池正负极焊到模块 `B+` / `B-`。
8. 将模块输出 `VO+` / `VO-` 焊到相机侧最终触点。
9. 用万用表确认输出电压、触点正负极和是否短路。
10. 对所有焊点和金属边缘做绝缘，再装入相机测试。

![装配剖面图](images/assembly-cross-section-detail.jpg)

## 开源许可

本项目使用 Creative Commons Attribution 4.0 International License 开源，详见 [LICENSE](LICENSE)。

Pentax 是 Ricoh Imaging Company, Ltd. 的商标。本项目为独立社区设计，与 Ricoh/Pentax 无隶属或官方背书关系。
