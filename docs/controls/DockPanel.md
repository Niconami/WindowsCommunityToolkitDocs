---
title: DockPanel
author: IbraheemOsama
description: Defines an area where you can arrange child elements either horizontally or vertically, relative to each other.
keywords: windows 10, uwp, windows community toolkit, uwp community toolkit, uwp toolkit, DockPanel, XAML Control, xaml
---

# DockPanel

The [DockPanel](/dotnet/api/microsoft.toolkit.uwp.ui.controls.dockpanel) control defines an area where you can arrange child elements either horizontally or vertically, relative to each other.

The DockPanel position child controls based on the child Dock property, you have 4 options to Dock, left (Default), right, top, bottom.
You can set DockPanel LastChildFill property to true if you want the last item added to the DockPanel to fill the rest empty space.

> [!div class="nextstepaction"]
> [Try it in the sample app](uwpct://Controls?sample=DockPanel)

## Syntax

```xaml
<Page ...
     xmlns:controls="using:Microsoft.Toolkit.Uwp.UI.Controls"/>

<controls:DockPanel Name="SampleDockPanel" Margin="2" Background="LightGray" LastChildFill="False" >
  <StackPanel Height="100" controls:DockPanel.Dock="Top" Background="Black"></StackPanel>
  <StackPanel Width="100" controls:DockPanel.Dock="Left" Background="Red"></StackPanel>
  <StackPanel Height="100" controls:DockPanel.Dock="Bottom" Background="Green"></StackPanel>
  <StackPanel Width="100" controls:DockPanel.Dock="Right" Background="Blue"></StackPanel>
</controls:DockPanel>
```

## Sample Output

![DockPanel animation](../resources/images/Controls/DockPanel.gif)

## Properties

| Property | Type | Description |
| -- | -- | -- |
| LastChildFill | bool | Gets or sets a value indicating whether the last child element within a DockPanel stretches to fill the remaining available space |
| Padding | Thickness | The dimensions of the space between the edge and its child as a Thickness value. Thickness is a structure that stores dimension values using pixel measures. |

## Sample Project

[DockPanel Sample Page Source](https://github.com/windows-toolkit/WindowsCommunityToolkit/tree/rel/7.1.0/Microsoft.Toolkit.Uwp.SampleApp/SamplePages/DockPanel). You can [see this in action](uwpct://Controls?sample=DockPanel) in the [Windows Community Toolkit Sample App](https://aka.ms/windowstoolkitapp).

## Requirements

| Device family | Universal, 10.0.16299.0 or higher |
| -- | -- |
| Namespace | Microsoft.Toolkit.Uwp.UI.Controls |
| NuGet package | [Microsoft.Toolkit.Uwp.UI.Controls](https://www.nuget.org/packages/Microsoft.Toolkit.Uwp.UI.Controls/) |

## API Source Code

* [DockPanel source code](https://github.com/windows-toolkit/WindowsCommunityToolkit/tree/rel/7.1.0/Microsoft.Toolkit.Uwp.UI.Controls.Primitives/DockPanel)
