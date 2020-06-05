
### Unity操作技巧：
	1.场景中，按住鼠标右键+方向键移动观察相机的同事按住shift，会加速移动
	2.场景中，选中某个物体按F键，会聚焦在该物体中，按两次，聚焦的同事让相机跟随
	3.按住数字2键 可以切换2D，3D视图



### GameObject: 
	
	uid: 物体在世界的ID


	Tag：标签
		1.	每一个GameObject 都有一个标签
		2.	GameObject.FindGameObjectWithTag("Test")   
			查找标签为Test的物体 

	Layer： 层
		1.	Layer与GameObject绑定，每个物体都有Layer
		2.	物理相关绝定是否发生碰撞
		3.	裁剪：与摄像机相关，是否发生该照相机是否投射到该Layer
			用	于显示, Light(光线)是否照射得到
		4.


	Component:
		1.Transform:	变换
		2.Render:		渲染
		3.Animation:	动画
		4.AI:			AI
		5.Light:		光线
		6.Camera:		相机
		7.Script:		脚本
		8.rigidBody: 	刚体



### 脚本和类名保持一致；
	语法解构

	using 命名空间
	class ClassName : MonoBehvaviour{


		[HideInInspactor]
		public fload s;		// 编辑器中隐藏；

		[Range(0,1)]		// 指定范围；
		public float b;		// 只有公有的字段在unity编辑看的见；

		public bool re;


		void Start()
		{

		}

		void Update()
		{

		}
	}

### 脚本的生命周期；
		1.	Awake()			//	脚本被载入是执行，用于游戏开始前进行初始化,如满足某种条件下执行this.enable=false   激活脚本；
		2.	OnEnable()  	//	当前对象变为可用或者激活状态时此函数调用	即this.enable = true; 
		3.	Start()			//	在Update函数第一次调用前调用；和Awake的不同是Start只在脚本实例被启用时调用；
		4.	Update()		//	处理
		5.	LateUpdate()	//	延迟更新，在Update函数被调用之后执行，如物体在Update中移动，跟随的物体放在LateUpdate中实现；
		6. 	FixedUpdate()	//	固定更新： 每个物理是将被调用一次，常用语物理计算，如对刚体添加力。 
							// 	修改更新频率Edit->Project Setting -> Time 在菜单栏中 Fixed Timestep 值，默认0.02；
	    7.	Reset()			//	没啥用； 重置数据；
		6.	OnDisable() 	// 	对象变为不可用或者游戏对象非激活状态时函数被调用；
		7.	OnDestory() 

















