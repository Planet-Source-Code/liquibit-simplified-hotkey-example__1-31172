<div align="center">

## Simplified Hotkey Example


</div>

### Description

Shows how to emplement a hotkey globally. This example uses the ` key (192).
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Liquibit](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/liquibit.md)
**Level**          |Beginner
**User Rating**    |3.6 (18 globes from 5 users)
**Compatibility**  |VB 3\.0, VB 4\.0 \(16\-bit\), VB 4\.0 \(32\-bit\), VB 5\.0, VB 6\.0
**Category**       |[Windows API Call/ Explanation](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/windows-api-call-explanation__1-39.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/liquibit-simplified-hotkey-example__1-31172/archive/master.zip)

### API Declarations

```
'Add To Module
Declare Function GetAsyncKeyState Lib "user32" (ByVal vKey As Long) As Integer
```


### Source Code

```
'Add To A Timer With An Interval Of 1
keyresult = GetAsyncKeyState(192)
 If keyresult = 0 Then Exit Sub
 If keyresult = -32767 Then
  MsgBox "The ` key was pressed."
 End If
```

