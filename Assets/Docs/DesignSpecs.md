# 核心文件夹结构

```
Assets/
├── 1_Scripts/                  # 所有C#脚本
│   ├── Core/                   # 核心逻辑（游戏管理器、全局事件）
│   ├── FireSimulation/         # 火灾模拟控制（PyroSim通信脚本）
│   ├── Database/               # MySQL数据库交互类（连接、查询、数据格式化）
│   ├── AI/                     # 深度学习接口（gRPC/REST客户端）
│   ├── UI/                     # 前端界面逻辑（按钮事件、数据展示）
│   └── Utils/                  # 工具类（文件读写、数学计算、扩展方法）
│
├── 2_Prefabs/                  # 预制体
│   ├── FireModels/             # 火灾模型预制体（建筑、火焰粒子系统）
│   ├── UI/                     # UI元素（面板、按钮、3D指示器）
│   └── Sensors/                # 虚拟传感器（温度/烟雾检测点）
│
├── 3_Scenes/                   # 场景文件
│   ├── Main.unity              # 主场景
│   ├── SimulationLab.unity     # 火灾模拟实验室场景
│   └── Debug.unity             # 调试专用场景
│
├── 4_Art/                      # 美术资源
│   ├── Models/                 # 3D模型（FBX/OBJ格式，需与PyroSim兼容）
│   ├── Materials/              # 材质球（火焰、烟雾、建筑材料）
│   ├── Textures/               # 贴图（漫反射、法线、遮罩）
│   └── Animations/             # 动画控制器（火灾蔓延动态效果）
│
├── 5_Plugins/                  # 第三方插件
│   ├── MySql.Data/             # MySQL Connector/NET的DLL文件
│   ├── Newtonsoft.Json/        # JSON解析库（用于API通信）
│   └── PyroSimBridge/          # PyroSim接口插件（如有SDK）
│
├── 6_Data/                     # 动态数据与配置文件
│   ├── Configs/                # JSON/XML配置文件（数据库IP、端口）
│   ├── PyroSimOutput/          # PyroSim生成的CSV数据（温度/烟雾记录）
│   └── AIData/                 # 深度学习模型的输入/输出缓存
│
├── 7_StreamingAssets/          # 需运行时访问的静态资源
│   └── FireScenarioPresets/    # 预设火灾场景参数（燃料分布、通风条件）
│
└── 8_Docs/                     # 项目文档（非必须，建议用外部仓库管理）
    ├── DesignSpecs.md          # 设计文档
    └── APIDocs/                # 接口文档（PyroSim/深度学习API说明）	
```