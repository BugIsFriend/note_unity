
RigidBody,Collider
    发生碰撞的两个物体必须带有Collider,发生碰撞的两个物体至少有一个带有刚体，
    发生碰撞的两个物体必须有相对运动。

    onTriggerEnter/Exit/Stay(Collider collider)   // 触发器
    onCollisionEnter/Exit/Stay(Collider collider) // 碰撞器

碰撞器是触发器的载体：触发器是碰撞起上的一个属性，
    当Is Trigger=false时，碰撞器根据物理引擎引发碰撞，产生碰撞的效果，可以调用OnCollisionEnter/Stay/Exit函数；
    当Is Trigger=true时，碰撞器被物理引擎所忽略，没有碰撞效果，可以调用OnTriggerEnter/Stay/Exit函数。


