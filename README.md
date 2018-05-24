# pew
![preview image](http://puu.sh/Ap75J.png)

#### alt+space launcher for steam built with electron.

Program runs in system-tray to listen for the alt+space shortcut and will open a small input field where you can start your steam games (or custom programs). It gets them from your steamapps folder which u might want to specify in the config file. Since v1.2.0 it includes an explorer file search and special tasks (math, google, urbandir) aswell. Bugs are expected because this is still in development but from my testing I found nothing *disturbing* yet. 

### Special Stuff
`>` - Steam Game Search
`#` - Code Search
`?` - Urban Dictionary Search
`\` - Google Search
(Not released yet)

[Download the latest version here](https://github.com/bakapear/pew/releases)

### Configuration / Custom Programs

After installing pew, navigate to `%appdata%/pew` where you'll find a `config.json` file containing some customization settings.
You can add custom programs to the search index or give nicknames to existing or custom programs.
```json
{
  "path": "C:/Program Files (x86)/Steam/steamapps",
  "nicks": {
    "440": [
      "tf2"
    ],
    "730": [
      "csgo"
    ]
  },
  "custom": [
    {
      "name": "osu!",
      "id": "%localappdata%/osu!/osu!.exe"
    },
    {
      "name": "Youtube",
      "nick": [
        "yt",
        "browser",
        "internet"
      ],
      "id": "chrome https://youtube.com/"
    }
  ]
}
```
