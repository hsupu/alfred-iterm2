# Alfred-iTerm2

## Guide

1. Open `Alfred Preferences` - `Features` - `Terminal / Shell`.
2. Change `Application` to `Customer`.
3. Use script as follow:

```applescript
on alfred_script(q)

-- set q to "ls" -- for debugtell application "System Events"	tell application "iTerm"		activate		set frontmost to true	end tell	keystroke "n" using {command down}	keystroke q	keystroke returnend tell

end alfred_script
```

## Usage

1. Open Alfred (`Alt+Space` as default).
2. Type `>` followed by your command.
3. Press `enter`.
4. Welcome star.
