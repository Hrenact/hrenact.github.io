# 一、准备工作

- 至少一个 HTC 1.0 / 2.0 基站（推荐两个）
- 你想要混搭的 PCVR 设备以及对应数量的接收器
- 软件 OpenVR-SpaceCalibrator 或 OpenVR-SpaceCalibrator-CN
- 连续校准用 HTC 1.0 / 2.0 / 3.0 Tracker 或 N7R Tundra Tracker（一个，可选）

# 二、基站兼容性

基站版本 | HTC 1.0 Traker | HTC 2.0 Traker | HTC 3.0 Traker | N7R Tundra Tracker | Index Knuckle 指虎 | HTC Vive 手柄 1.0 | HTC Vive 手柄 2.0
-- | -- | -- | -- | -- | -- | -- | --
HTC 1.0 基站 | √ | √ | √ | √ | √ | √ | √
HTC 2.0 基站 | × | √ | √ | √ | √ | × | √

> [!CAUTION]
> 虽然 N7R Tundra Tracker 在官网标明支持 HTC 1.0 基站，但是这里的支持仅限于能被基站识别。要达到稳定的追踪效果需要非常苛刻的条件，慎重考虑！

# 三、设备常见规格

设备名称 | 固定接口类型 | 固定接口方位 | 供电 / 充电接口类型
-- | -- | -- | --
HTC 1.0 基站 | 1/4 英寸螺丝口 | 底面 / 背面 | DC 12V 2.5A 5.5*1.25mm 圆孔插头
HTC 2.0 基站 | 1/4 英寸螺丝口 | 底面 / 背面 | DC 12V 2.5A 5.5*1.25mm 圆孔插头
HTC 1.0 Traker | 1/4 英寸螺丝口 | 底面 | Micro USB
HTC 2.0 Traker | 1/4 英寸螺丝口 | 底面 | Micro USB
HTC 3.0 Traker | 1/4 英寸螺丝口 | 底面 | Type-C
N7R Tundra Tracker | 可更换式 1/4 英寸螺丝口 | 底面 | Type-C
Index Knuckle 指虎 | 无 | 无 | Type-C
HTC Vive 手柄 1.0 | 无 | 无 | Micro USB
HTC Vive 手柄 2.0 | 无 | 无 | Micro USB

> [!NOTE]
> 表格中的“1/4 英寸螺丝口”为英制单位。如果你担心，可以直接搜索“1/4 相机螺丝口”。

# 四、基站规格

基站版本 | 照射距离（单个 / 多个） | 最大数量 | 注意事项
-- | -- | -- | --
1.0 | 3.5 米 / 5 米 | 2 个 | 安装 2 个基站时，需确保基站能相互“看见”
2.0 | 7 米 / 10 米 | 4 个 | 避免安装环境出现强光源

> [!WARNING]
> HTC 1.0 基站对于最近距离的要求为 0.5 米，小于此距离的 Lighthouse 设备有可能会造成无法识别的问题。

# 五、配件注意事项

HTC 1.0 基站在除了供电接口外，还有一个特殊的接口为“同步线接口”。在特殊情况导致基站无法同步时，可以通过在基站之间连接“同步数据线”来恢复同步。

购买除了基站以外的其它 Lighthouse 设备时，需注意是否包含接收器。如不包含，你需要单独购买或者使用数据线连接设备与电脑才能定位。

# 六、安装基站

这里将使用图像粗略的演示基站应如何安装。

房间规模：

`Gmeek-html<img src="https://hrenact.github.io/RoomMode.drawio.png">`

或

`Gmeek-html<img src="https://hrenact.github.io/RoomMode2.drawio.png">`

客厅规模：

`Gmeek-html<img src="https://hrenact.github.io/LivingroomMode.drawio.png">`

总之，我们按照以下几点摆放基站即可：

- 将基站照射范围覆盖游戏区域
- 将基站安装在房间高处并向下倾斜 25度 至 35度
- 避免基站照射范围出现高反射率物体（例：镜子）

在你安装好基站并开启 SteamVR 后，基站不会显示在 SteamVR 界面中。当在基站照射范围内出现已配对 / 使用数据线连接至电脑的 Lighthouse 设备时，基站将自动显示。

> [!WARNING]
> 在基站通电时请勿大幅度移动或磕碰基站，这可能会导致基站损坏！

# 七、设置基站频道

## 1. HTC 1.0 基站

- 不使用同步数据线：
按下定位器背面的频道按钮，将一个定位器设为频道​ b ，另一个设为频道​ c 。

- 使用同步数据线：
按下定位器背面的频道按钮，将一个定位器设为频道 ​‍A ，另一个设为频道 b 。

你可以在基站正面看到对应的频道模式指示灯亮起。亦或者将鼠标移动至 SteamVR 的基站图标上并稍作等待，即可在浮现的窗口中查看基站当前频道。

## 2. HTC 2.0 基站

对于 HTC 2.0 基站，SteamVR 会自动设置基站的频道。如果你的 Lighthouse 设备出现频繁丢追或者 SteamVR 虚拟空间内的基站数量与现实基站数量不对应，则有可能遇到了频道冲突的情况。

将鼠标移动至 SteamVR 的基站图标上并稍作等待，即可在浮现的窗口中查看基站当前频道。如果有超过一个基站的频道数相同，则需要你手动切换基站频道来恢复正常。

在基站电源接口的上方，有一个小孔，作用为手动切换频道。使用手机卡针或者掰直的回形针捅入小孔，在触底后短按一下，此时就已将完成手动切换基站频道。

> [!NOTE]
> 你应该在基站通电的情况下进行更换频道操作，建议你使用一手扶 / 拿好基站一手进行更换频道的操作，避免造成不必要的损失！

# 八、添加 Lighthouse 设备

将接收器插入电脑的 USB 2.0 或更高规模的 USB 接口，并启动 SteamVR。

点击 SteamVR 左上角的菜单，打开下拉菜单。将鼠标移动至“设备”，稍做等待，在浮现的窗口中点击“配对控制器”，弹出“选择您的控制器类型”窗口。

`Gmeek-html<img src="https://hrenact.github.io/SteamVR.png">`

Controller Pairing：

`Gmeek-html<img src="https://hrenact.github.io/AddController.png">`

选择对应的设备，按照提示完成配对，成功后将在 SteamVR 界面出现你刚刚添加的设备。

你应该每次只插入一个接收器并配对一个设备，在配对完成后长按设备的系统键直到LED灯熄灭，意味着设备已关机。此时再插入一个接收器并配对新设备，重复此过程直到完成所有设备的添加。

如果你使用的是 Tundra SteamVR 通用多合一接收器（Tundra SteamVR Super Wireless Dongle），建议你只配对“接收器最大配对数量 - 1”个数量。

在配对或配对完成后选择“配对另一个控制器”时，如果出现“请关闭您现有控制器中的一个”字样，请检查是否插入了数量充足的接收器并确保接口牢固。如果不起作用，请转到 SteamVR x.x.x → 开发者 → 开发者设置 并点击“移除所有 SteamVR USB 设备”并从头开始重新配对。

> [!NOTE]
> 你可以先只添加一个 Tracker ，方便在连续校准章节中快速找到需要作为连续校准用的目标设备。

# 九、校准 Lighthouse 设备

## 1. 安装校准软件

下载并安装软件 [OpenVR-SpaceCalibrator](https://github.com/hyblocker/OpenVR-SpaceCalibrator/releases/tag/v1.5)，或者选择它的汉化版 [OpenVR-SpaceCalibrator-CN](https://github.com/Hrenact/OpenVR-SpaceCalibrator-CN/releases/tag/v1.5.1)。此教程使用汉化版来演示。

如果你安装的原始版本为 v1.5 ，你可以参照此教程中的汉化版截图来操作。

打开 SteamVR ，确认你的头戴设备已连接至 SteamVR 。OpenVR-SpaceCalibrator 会跟随 SteamVR 一并启动，如果没有，请手动双击桌面的快捷方式来开启。

软件界面：

`Gmeek-html<img src="https://hrenact.github.io/SpaceCalibratorCN.png">`

> [!NOTE]
> 初次安装的 OpenVR-SpaceCalibrator 只会显示“开始校准”选项，你需要进行一次手动校准才能解锁其它选项。

## 2. 手动校准

手动校准需要将“主设备”选择为一体机的左或者右手柄，并将“副设备”选择为对应的 Lighthouse PCVR 的左或者右指虎手柄。

以 Pico 4 举例：

`Gmeek-html<img src="https://hrenact.github.io/P4Left.png">`

或

`Gmeek-html<img src="https://hrenact.github.io/P4Right.png">`

选择合适的“校准速度”，此选项仅影响手动校准时校准的时长。越长的校准时长意味着越多的校准数据，也意味着位置越准确。

将你选择的设备握紧在一起，确保在校准过程中它们的相对位置不会发生偏移。

单击“开始校准”，尽可能的移动和旋转你选择的设备（例如：画8字），确保软件获取到足够的位置信息。

在进度条未达到 100% 之前，你应该一直保持着握紧并移动和旋转设备的状态。

> [!NOTE]
> 如果你拥有连续校准用 Tracker，可以使用连续校准的设备方案进行手动校准。注意：未佩戴的头显有可能会进入睡眠模式并关闭追踪，你需要在佩戴头显的情况下进行校准。

在校准成功后，将在进度条下方出现“Finshed calibration, profile saved”，单击下方的“Close”按钮来返回主界面。

`Gmeek-html<img src="https://hrenact.github.io/Finished.png">`

此时，你的 PCVR 设备在 SteamVR 界面的位置将会与现实位置同步。

> [!WARNING]
> 如果未出现“Finshed calibration, profile saved”或出现其它文本，则为校准失败，你应该点击“Close”按钮并重新校准。

## 3. 连续校准

使用连续校准方案时，VRChat 会默认打开 FBT 支持模式。如有需要，你可以在小设置菜单中关闭全身追踪。

连续校准需要将“主设备”选择为一体机的头显，并将“副设备”选择为固定在头戴式设备上的 Tracker。

以 Pico 4 举例：

`Gmeek-html<img src="https://hrenact.github.io/P4Tracker.png">`

点击“连续校准”来进入到连续校准界面。

连续校准主要界面：

`Gmeek-html<img src="https://hrenact.github.io/AlwaysCalibrator.png">`

简单介绍一下我们需要用到的功能：

- 取消连续校准：单击后将退出连续校准并回到软件主界面
- 隐藏混搭追踪器：勾选后将在 VRChat 校准全身追踪时隐藏此追踪器
- 保持自动校准：勾选后软件将一直在后台校准设备位置

对于普通用户，勾选“隐藏混搭追踪器”和“保持自动校准”即可。

勾选后，带上头显并在房间内走动，软件将收集数据并将 SteamVR LightHouse 设备位置与现实位置同步。

> [!NOTE]
> 目标设备的 Tracker 名称会因实际型号而异，演示型号为 HTC 3.0 Traker 。如果你怕选错设备，可以暂时只开启连续校准用 Tracker ，配置好连续校准参数后再逐一开启其它设备。

# 十、额外设备推荐

这里会陈列一些对混搭玩家有用的商品，仅供参考。它们都是使用手机浏览器访问并跳转至第三方应用的链接。

- USB 拓展坞
https://m.tb.cn/h.gkkbKa9mUFLfbu9?tk=22ws33ZTMlB

- USB 充电坞
https://m.tb.cn/h.gPQ2Lsg3TPBAPKb?tk=lw7b33Z5oLx

- Type-C 充电线
https://m.tb.cn/h.gPQV8uuwNlWcMFA?tk=O3BX33ZSYoj

- USB 2.0 延长线
https://m.tb.cn/h.gkDqv36zXUVJ4J7?tk=UAMx330zbQw

- 一体机 Tracker 固定底座
https://m.tb.cn/h.gkke7vI?tk=JAch33ZQ0IQ