# WINDHAWK Settings

## Prereqs:
- Windows 11
- [Windhawk](https://windhawk.net/)

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

## taskbar-tray-system-icon-tweaks
```json
{
  "hideVolumeIcon": 0,
  "hideNetworkIcon": 0,
  "hideBatteryIcon": 0,
  "hideMicrophoneIcon": 1,
  "hideGeolocationIcon": 0,
  "hideStudioEffectsIcon": 0,
  "hideLanguageBar": 1,
  "hideLanguageSupplementaryIcons": 0,
  "hideBellIcon": "whenInactiveAndNoDnd",
  "showDesktopButtonWidth": 12
}
```

## [WinDock](https://github.com/DarkionAvey/windhawk-taskbar-centered-condensed)
```json
{
	"TaskbarHeight": 56,
	"TaskbarIconSize": 24,
	"TaskbarButtonSize": 52,
	"TaskbarOffsetY": 8,
	"TrayTaskGap": 8,
	"TaskbarBackgroundHorizontalPadding": 0,
	"FullWidthTaskbarBackground": 0,
	"IgnoreShowDesktopButton": 0,
	"TaskbarCornerRadius": 8,
	"TaskButtonCornerRadius": 4,
	"FlatTaskbarBottomCorners": 0,
	"CustomizeTaskbarBackground": 1,
	"TaskbarBackgroundOpacity": 100,
	"TaskbarBackgroundTint": 0,
	"TaskbarBackgroundLuminosity": 50,
	"TaskbarBorderOpacity": 5,
	"TaskbarBorderColorHex": "#ffffff",
	"TaskbarBorderThickness": 8,
	"AppsDividerThickness": 8,
	"AppsDividerVerticalScale": 40,
	"AppsDividerAlignment": "left",
	"DividedAppNames": "File Explorer",
	"TrayAreaDivider": 1,
	"StyleTrayArea": 1,
	"TrayIconSize": 16,
	"TrayButtonSize": 30,
	"MoveFlyoutStartMenu": 1,
	"MoveFlyoutControlCenter": 1,
	"MoveFlyoutNotificationCenter": 0,
	"AlignFlyoutInner": 1
}
```
