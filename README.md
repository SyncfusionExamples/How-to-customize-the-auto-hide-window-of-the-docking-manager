# How-to-customize-the-auto-hide-window-of-the-docking-manager

This sample demonstrates how to customize the auto-hide (side) panel and its header in Syncfusion WPF DockingManager. You can tune background, border brush, border thickness, and the panel size to match your application’s theme. The same styling can be applied consistently to both the side container and the auto-hide tab headers to create a coherent look.

## Customization 

The side panel and side panel header can be customized by applying its Background, BorderBrush, BorderThickness and SidePanelSize through SidePanelBackground, SidePanelBorderBrush, SidePanelBorderThickness, SidePanelSize properties of the DockingManager. You can also refer to this sample which demonstrate the side panel customization.

## Code snippet

### XAML:
``` xml
<syncfusion:DockingManager SidePanelBackground="Brown"
                           SidePanelBorderBrush="Yellow" SideItemsBackground="Green"
                           SidePanelBorderThickness="2,2,2,2" SideItemsBorderBrush="BlueViolet" SidePanelSize="40">

<ContentControl syncfusion:DockingManager.Header="SolutionExplorer" syncfusion:DockingManager.State="AutoHidden" />

<ContentControl syncfusion:DockingManager.Header="ToolBox" />

</syncfusion:DockingManager>
```

### C#:

``` csharp
//Set Customization colors
SyncDockingManager.SidePanelBackground = new SolidColorBrush(Colors.Brown);
SyncDockingManager.SidePanelBorderBrush = new SolidColorBrush(Colors.Yellow);
SyncDockingManager.SideItemsBackground = new SolidColorBrush(Colors.Green);
SyncDockingManager.SideItemsBorderBrush = new SolidColorBrush(Colors.Violet);
SyncDockingManager.SidePanelBorderThickness = new Thickness(2, 2, 2, 2);
SyncDockingManager.SidePanelSize = 40;
```
The screenshot below displays the customized autohide window.
![Customized autohide window](auto-hide-window.png)

## What you’ll learn:

- Apply SidePanelBackground for the strip surface and SideItemsBackground for the tab headers
- Add visual separation using SidePanelBorderBrush and SidePanelBorderThickness
- Tune SidePanelSize to define how thick the side strip appears on the docking edge
- Configure settings in XAML and optionally adjust at runtime in code

## Notes:

- SidePanelBackground colors the auto-hide strip that hosts the side tabs.
- SideItemsBackground applies to the tab headers within the strip.
- SidePanelBorderBrush and SidePanelBorderThickness add definition to the strip edges.
- SidePanelSize controls strip thickness and impacts perceived density and hit targets.
