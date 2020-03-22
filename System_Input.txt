
1.Input:系统输入

  InputManager

  Input.GetKey()
  Input.GetButton()        //返回bool
  Input.GetButtonDown()    //返回bool
  Input.GetButtonUp()      //返回bool

  Input.getAxis()           // 返回0-1的小数点， 返回由Gravity,sensitivit控制的运动区间 
  Input.getAxisRaw()        // 

  Input.OnMouseEnter()      // 但鼠标进入GUIElement会被调用
  Input.OnMouseOver()       // 但鼠标悬浮在GUIElement时会被调用
  Input.OnMouseUp()         // 但鼠标悬浮在GUIElement时会被调用
  Input.OnMouseDown()       // 但鼠标悬浮在GUIElement时会被调用
