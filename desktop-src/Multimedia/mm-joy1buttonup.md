---
title: MM_JOY1BUTTONUP message (Mmsystem.h)
description: The MM\_JOY1BUTTONUP message notifies the window that has captured joystick JOYSTICKID1 that a button has been released.
ms.assetid: 37f0f87a-4805-4cec-9c0c-9d6b36a3ff0d
keywords:
- MM_JOY1BUTTONUP message Windows Multimedia
topic_type:
- apiref
api_name:
- MM_JOY1BUTTONUP
api_location:
- Mmsystem.h
api_type:
- HeaderDef
ms.topic: reference
ms.date: 05/31/2018
---

# MM\_JOY1BUTTONUP message

The **MM\_JOY1BUTTONUP** message notifies the window that has captured joystick JOYSTICKID1 that a button has been released.


```C++
MM_JOY1BUTTONUP 
fwButtons = wParam; 
xPos = LOWORD(lParam); 
yPos = HIWORD(lParam); 
```



## Parameters

<dl> <dt>

<span id="fwButtons"></span><span id="fwbuttons"></span><span id="FWBUTTONS"></span>*fwButtons*
</dt> <dd>

Identifies the button that has changed state and the buttons that are pressed. It can be one of the following:



| Requirement | Value |
|-----------------|-------------------------------------------|
| JOY\_BUTTON1CHG | First joystick button has changed state.  |
| JOY\_BUTTON2CHG | Second joystick button has changed state. |
| JOY\_BUTTON3CHG | Third joystick button has changed state.  |
| JOY\_BUTTON4CHG | Fourth joystick button has changed state. |



 

and one or more of the following:



| Requirement | Value |
|--------------|------------------------------------|
| JOY\_BUTTON1 | First joystick button is pressed.  |
| JOY\_BUTTON2 | Second joystick button is pressed. |
| JOY\_BUTTON3 | Third joystick button is pressed.  |
| JOY\_BUTTON4 | Fourth joystick button is pressed. |



 

</dd> <dt>

<span id="xPos"></span><span id="xpos"></span><span id="XPOS"></span>*xPos*
</dt> <dd>

The x-coordinates of the joystick relative to the upper left corner of the client area.

</dd> <dt>

<span id="yPos"></span><span id="ypos"></span><span id="YPOS"></span>*yPos*
</dt> <dd>

The y-coordinate of the joystick relative to the upper left corner of the client area.

</dd> </dl>

## Requirements



| Requirement | Value |
|-------------------------------------|-----------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 2000 Professional \[desktop apps only\]<br/>                                                |
| Minimum supported server<br/> | Windows 2000 Server \[desktop apps only\]<br/>                                                      |
| Header<br/>                   | <dl> <dt>Mmsystem.h (include Windows.h)</dt> </dl> |



## See also

<dl> <dt>

[Joysticks](joysticks.md)
</dt> <dt>

[Multimedia Joystick Messages](multimedia-joystick-messages.md)
</dt> </dl>

 

 





