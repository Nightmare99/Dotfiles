# WINDHAWK Settings

## Prereqs:
- Windows 11
- Windhawk

## windows-11-taskbar-styler
```json
{
  "theme": "DockLike",
  "controlStyles[0].target": "Taskbar.TaskbarFrame > Grid#RootGrid",
  "controlStyles[0].styles[0]": "Margin=0,1,0,3",
  "styleConstants[0]": "",
  "resourceVariables[0].variableKey": "",
  "resourceVariables[0].value": "",
  "controlStyles[0].styles[1]": "CornerRadius=8",
  "controlStyles[1].target": "Grid#RootGrid",
  "controlStyles[1].styles[0]": "Background:=<WindhawkBlur BlurAmount=\"30\" TintColor=\"#4D000000\" />",
  "controlStyles[2].target": "Grid#SystemTrayFrameGrid",
  "controlStyles[2].styles[0]": "Background:=<WindhawkBlur BlurAmount=\"30\" TintColor=\"#4D000000\" />"
}
```

## windows-11-start-menu-styler
```json
{
  "theme": "Fluid",
  "disableNewStartMenuLayout": 0,
  "controlStyles[0].target": "",
  "controlStyles[0].styles[0]": "",
  "webContentStyles[0].target": "",
  "webContentStyles[0].styles[0]": "",
  "webContentCustomJs": "",
  "styleConstants[0]": "",
  "resourceVariables[0].variableKey": "",
  "resourceVariables[0].value": ""
}
```

## taskbar-icon-size
```json
{
  "TaskbarHeight": 56,
  "IconSize": 32,
  "TaskbarButtonWidth": 52,
  "IconSizeSmall": 16,
  "TaskbarButtonWidthSmall": 32
}
```

## taskbar-auto-hide-when-maximized
```json
{
  "mode": "intersected",
  "foregroundWindowOnly": 0,
  "excludedPrograms[0]": "",
  "primaryMonitorOnly": 0,
  "oldTaskbarOnWin11": 0
}
```

## taskbar-auto-hide-speed
```json
{
  "showSpeedup": 250,
  "hideSpeedup": 250,
  "frameRate": 240,
  "oldTaskbarOnWin11": 0
}
```