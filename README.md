# goautoit
golang invoke autoit function through AutoItX3.dll

## Install

```golang
go get -u github.com/ajmandourah/goautoit
```
Either download the latest version of the autoit DLL or use the included one. 

Put the DLL in the same path as your project. 
## Example

- open notepad
- type some string into notepad, eg: **"hello world"**
- close notepad without saving

```golang
goautoit.Run("notepad.exe")
goautoit.WinWait("Untitled")
goautoit.Send("hello world")
goautoit.WinClose("Untitled")
```
