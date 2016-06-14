Tuesday, June 14, 2016
### An Object-Oriented Approach to Programming Logic and Design
#### Programming Logic and Design
###### Lesson 5
###### Understanding Desktop Applications

###### Understanding Windows Form Applications
- small client app consisting of on or more forms that display a visual interface to the user

`NOTE: Windows Forms good way to learn C#`

- Windows Forms Event Model uses the .NET framework delegates

`NOTE: partial class is a class broken up into to parts, but comes together when compiled`

`NOTE: constructor (initializes) has the same name as the class`

```csharp
public partial class InheritedForm: Form1
{
  public InheritedForm(){
    // constructor, has the same name as the class
    // can have multiple constructors but must have a different `signature`
  }
}

```

- MDI Multiple Document Interface Applications
  - multiple child windows under a single parent
  - share a single application menu and toolbar
  - single document interface (SDI) applications, each window contains its own menu and toolbar
  - `IsMdiContainer` set property to true, to create an MDI application
  - `MdiParent` property to refer to the parent property

- Console-based Applications
  - no GUI, uses text-mode
  - require no user interface

-  Windows Service Applications
  - apps that runs in the background, no GUI
  - long-running programs that run in the background
  - can be started, paused, restarted and stopped
  - can be set to start automatically
  - play important role in enterprise application architecture


View running services
  - Computer Management => Services and Applications => Services


Creating a Windows Service Applications (may have to search for it in Visual Studio)
