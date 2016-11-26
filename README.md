# Alfred-iTerm2

## Guide

1. Open `Alfred Preferences` - `Features` - `Terminal / Shell`.
2. Change `Application` to `Customer`.
3. Use script as follow:

```applescript
on alfred_script(q)

-- for debug
-- set q to "ls"
tell application "System Events"
    tell application "iTerm2"
        create window with default profile
        delay 0.5
        tell current session of current window
            write text q
        end tell
    end tell
end tell

end alfred_script
```

## Usage

1. Open Alfred (`Alt+Space` as default).
2. Type `>` followed by your command.
3. Press `enter`.
4. Welcome star.
