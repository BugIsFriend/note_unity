### 继承体系:
        Object: 
                1.GameObject:
                2.Component:
                        1.Behavior                      继承自Component
                                    1.Animation         继承自Behavior
                                    2.Camera            继承自Behavior
                                    3.Light             继承自Behavior
                                    4.MonoBehaviour     继承自Behavior
                        2.Renderer                      继承自Component
                                    1.MeshRenderer:
                                    2.PariticleRenderer:
                        3.Collider
                        4.Joint
                        5.MeshFilter
                        6.RigidBody
                        7.Transform
                3.Material:
                4.Mesh:
                5.Texture:
                6.Shader:



Debug.Log()
Debug.LogError()
Debug.Log


### 脚本的响应事件和组件的访问：脚本都继承自MonoBehaviour类
    1.脚本的生命周期：
    2.脚本的响应事件和组件的访问
         MonoBehaviour事件响应：
                             1.启动函数：Reset(),Awake(),Start()
                             2.刷新函数：FixUpdate(),Update(),LateUpdate()
                             3.交互函数：分为一下几种
                                        物理响应函数： OnTriggerEnter/Exit/Stay()     当碰撞体发生出发被调用/碰撞体没有碰撞被调用／碰撞体碰撞过程中被调用
                                                     OnCollisionEnter/Exit/Stay()
                                                     OnConTrollerColliderHit()
                                                     OnJoinBreak()
                                                     OnParicleCollision()

                                        鼠标Input函数：  OnMouseEnter/Over/Exit/Down/Drag()

                                        渲染Rendering:   OnGUI()/OnDrawGizmos()
                                        对象Object:      OnEnable()/OnDisable()/OnDestroy()
                                        程序Application: OnApplicationsPause/Focus/Quit()

                                        网络Network:     OnPlayerConnected／Disconnected()
                                                        OnServerInitialized()
                                                        OnConnectedToServer()

                                        动画Animator:   OnAnimatorMove():
                                                        OnAnimatorIK()
                                        动画Audio:      OnAudioFilterRead()  

    3.组件的添加与访问：
        getComponent<ComponentType>()   // 通过类型获取组件   
        getComponent("ComponentName")   // 通过名字获取脚本
                                     

                                                         


                 

