# 准备工作

- 至少一个 HTC 1.0 / 2.0 / 3.0 Tracker 或 N7R Tundra Tracker （即连续校准用 Tracker）
- 至少一个 HTC 1.0 / 2.0 基站
- 你想要混搭的 PCVR 设备以及对应数量的 接收器 / 加密狗
- 软件 OpenVR-SpaceCalibrator / OpenVR-SpaceCalibrator-CN

# 基站兼容

基站版本 | HTC 1.0 Traker | HTC 2.0 Traker | HTC 3.0 Traker | N7R Tundra Tracker | Index 指虎
-- | -- | -- | -- | -- | --
HTC 1.0 基站 | √ | √ | × | √ | √
HTC 2.0 基站 | × | √ | √ | √ | √

# 设备规格

设备名称 | 接口类型 | 接口方位 | 供电/充电接口
-- | -- | -- | --
HTC 1.0 基站 | 1/4 英寸螺丝口 | 底面 / 背面 | DC 12V 2.5A 5.5*1.25mm 圆孔插头
HTC 2.0 基站 | 1/4 英寸螺丝口 | 底面 / 背面 | DC 12V 2.5A 5.5*1.25mm 圆孔插头
HTC 1.0 Traker | 1/4 英寸螺丝口 | 底面 | Micro USB
HTC 2.0 Traker | 1/4 英寸螺丝口 | 底面 | Micro USB
HTC 2.0 Traker | 1/4 英寸螺丝口 | 底面 | Type-C
N7R Tundra Tracker | 可更换式 1/4 英寸螺丝口 | 底面 | Type-C
Index 指虎 | 无 | 无 | Type-C

> [!NOTE]
> 表格中的“1/4 英寸螺丝口”为英制单位。如果你担心，可以直接搜索“1/4 相机螺丝口”。

# 闲鱼注意

HTC 1.0 基站在除了供电接口外，还有一个特殊的接口为“同步线接口”。在特殊情况导致基站无法同步时，可以通过在基站之间连接“同步数据线”来恢复同步。
在闲鱼购买 Tracker 或 指虎 时，需注意是否包含 接收器 / 加密狗。如不包含，你需要单独购买或者使用数据线连电脑才能定位。

# 安装基站

这里将使用字符粗略的演示基站如何安装。其中，箭头代表了基站的朝向。

房间规模：
┌──────────────┐
门           ↙│
门             │
│    床床床   电│
│衣  床床床   脑│
│柜↗床床床   桌│
└──────────────┘

客厅规模：
↘
   ┌┄┄┄┄┐
   ┆游玩┆
   ┆区域┆
   └┄┄┄┄┘
           ↖

总之，我们按照以下几点摆放基站即可：
- 按照对角线摆放基站
- 将基站照射范围覆盖游戏区域
- 将基站安装在房间高处并向下倾斜 20度 至 45度
- 避免基站照射范围出现高反射率物体（例：镜子）

> [!WARNING]
> 在基站通电时请勿大幅度移动或磕碰基站，这可能会导致基站损坏！

# 添加设备

将 接收器 / 加密狗 插入电脑的 USB 接口，并启动 SteamVR。

点击 SteamVR 左上角的菜单，打开下拉菜单。将鼠标移动至“设备”，稍做等待，在浮现的窗口中点击“配对控制器”，弹出“选择您的控制器类型”窗口。

选择对应的设备，按照提示完成配对，成功后将在 SteamVR 界面出现你刚刚添加的设备。

# 连续校准

下载并安装软件 [OpenVR-SpaceCalibrator](https://github.com/hyblocker/OpenVR-SpaceCalibrator/releases/tag/v1.5)；
或者选择它的汉化版 [OpenVR-SpaceCalibrator](https://github.com/Hrenact/OpenVR-SpaceCalibrator-CN/releases/tag/v1.5.1)。