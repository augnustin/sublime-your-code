![Sublime Text](./assets/logo-sublime-3.png)

# Sublime 
# your code

Presentation available at    
[http://aug-riedinger.github.io/sublime-tips](http://aug-riedinger.github.io/sublime-tips)
--
## Access your code

#### Among the project

|                                    | ![Linux](./assets/linux-logo.png) | ![Mac](./assets/OS_X-Logo.png) |
|:----------------------------------:|:--------------------------------:|:---------------------:|
|     Access a file with filename    |            ![Ctrl](./assets/keyboard/ctrl.png) + ![P](./assets/keyboard/p.png)            |       ![Cmd](./assets/keyboard/cmd.png) + ![P](./assets/keyboard/p.png)       |
| Access a file with snippet of code |        ![Ctrl](./assets/keyboard/ctrl.png) + ![Shift](./assets/keyboard/shift.png) + ![F](./assets/keyboard/f.png)        |   ![Cmd](./assets/keyboard/cmd.png) + ![Shift](./assets/keyboard/shift.png) + ![F](./assets/keyboard/f.png)  |

--
## Access your code

#### Within the opened file
|                                    | ![Linux](./assets/linux-logo.png) | ![Mac](./assets/OS_X-Logo.png) |
|:----------------------------------:|:--------------------------------:|:-----------------------------:|
|     Access line number             | ![Ctrl](./assets/keyboard/ctrl.png) + ![G](./assets/keyboard/g.png) | ![Ctrl](./assets/keyboard/ctrl.png) + ![G](./assets/keyboard/g.png)       |
|     Access symbol                  |            ![Ctrl](./assets/keyboard/ctrl.png) + ![R](./assets/keyboard/r.png)            |       ![Cmd](./assets/keyboard/cmd.png) + ![R](./assets/keyboard/r.png)       |
|     Move to next word *             | ![Ctrl](./assets/keyboard/ctrl.png) + ![Right](./assets/keyboard/cursor-right.png) | ![Cmd](./assets/keyboard/cmd.png) + ![Right](./assets/keyboard/cursor-right.png)       |
|     Move to previous word *             | ![Ctrl](./assets/keyboard/ctrl.png) + ![Left](./assets/keyboard/cursor-left.png) | ![Cmd](./assets/keyboard/cmd.png) + ![Left](./assets/keyboard/cursor-left.png)       |
|     Move to end of line *             | ![Ctrl](./assets/keyboard/ctrl.png) + ![End](./assets/keyboard/end.png) | ![Cmd](./assets/keyboard/cmd.png) + ![End](./assets/keyboard/end.png)       |
|     Move to beginning of line *             | ![Ctrl](./assets/keyboard/ctrl.png) + ![Home](./assets/keyboard/home.png) | ![Cmd](./assets/keyboard/cmd.png) + ![Home](./assets/keyboard/home.png)       |

> \* Press ![Shift](./assets/keyboard/shift.png) to keep selection 

--
## Move your code

|                   | ![Linux](./assets/linux-logo.png) |  ![Mac](./assets/OS_X-Logo.png) |
|:-----------------:|:--------------------------------:|:------------------------------:|
|  Duplicate a line |        ![Ctrl](./assets/keyboard/ctrl.png) + ![Shift](./assets/keyboard/shift.png) + ![D](./assets/keyboard/d.png)        |       ![Cmd](./assets/keyboard/cmd.png) + ![Shift](./assets/keyboard/shift.png) + ![D](./assets/keyboard/d.png)       |
| Move up line |  ![Ctrl](./assets/keyboard/ctrl.png) + ![Shift](./assets/keyboard/shift.png) + ![Up](./assets/keyboard/cursor-up.png)  | ![Ctrl](./assets/keyboard/ctrl.png) + ![Cmd](./assets/keyboard/cmd.png) + ![Up](./assets/keyboard/cursor-up.png) |
| Move down line |  ![Ctrl](./assets/keyboard/ctrl.png) + ![Shift](./assets/keyboard/shift.png) + ![Down](./assets/keyboard/cursor-down.png)  | ![Ctrl](./assets/keyboard/ctrl.png) + ![Cmd](./assets/keyboard/cmd.png) + ![Down](./assets/keyboard/cursor-down.png) |
|  Move right  |          ![Tab](./assets/keyboard/tab.png)         |         ![Tab](./assets/keyboard/tab.png)        |
|  Move left  |          ![Shift](./assets/keyboard/shift.png)+![Tab](./assets/keyboard/tab.png)         |         ![Shift](./assets/keyboard/shift.png)+![Tab](./assets/keyboard/tab.png)        |
|   Comment/Uncomment a line  |        ![Ctrl](./assets/keyboard/ctrl.png) + ![Shift](./assets/keyboard/shift.png) + ![Slash](./assets/keyboard/keypad-slash.png)        |       ![Cmd](./assets/keyboard/cmd.png) + ![Slash](./assets/keyboard/keypad-slash.png)       |

> You barely never need multiple-line comments

--
## Multiple Edits

|                                | ![Linux](./assets/linux-logo.png) | ![Mac](./assets/OS_X-Logo.png) |
|:------------------------------:|:--------------------------------:|:-----------------------------:|
|     Create multiple cursor     |          ![Ctrl](./assets/keyboard/ctrl.png) + Click          |         ![Cmd](./assets/keyboard/cmd.png) + Click        |
|   Select multiple occurrences  |            ![Ctrl](./assets/keyboard/ctrl.png) + ![D](./assets/keyboard/d.png)            |           ![Cmd](./assets/keyboard/cmd.png) + ![D](./assets/keyboard/d.png)          |
|      Undo select operation     |            ![Ctrl](./assets/keyboard/ctrl.png) + ![U](./assets/keyboard/u.png)            |    ![Cmd](./assets/keyboard/cmd.png) + ![U](./assets/keyboard/u.png)                           |
| Break line in multiple cursors |            ![Ctrl](./assets/keyboard/ctrl.png) + ![L](./assets/keyboard/l.png)            |           ![Cmd](./assets/keyboard/cmd.png) + ![L](./assets/keyboard/l.png)          |
| Break line in multiple cursors |        ![Ctrl](./assets/keyboard/ctrl.png) + ![Shift](./assets/keyboard/shift.png) + ![L](./assets/keyboard/l.png)        |       ![Cmd](./assets/keyboard/cmd.png) + ![Shift](./assets/keyboard/shift.png) + ![L](./assets/keyboard/l.png)      |

--
## Customize

Add a reindent shortcut
```
{ 
  "keys": ["f10"], 
  "command": "reindent", 
  "args": {
    single_line": false
  }
}
```

--
## Usefull Plugins

Install [plugins](https://sublime.wbond.net/installation): ![Ctrl](./assets/keyboard/ctrl.png) + ![Shift](./assets/keyboard/shift.png) + ![P](./assets/keyboard/p.png) --> `Install Package`

- [Sidebar enhancement](https://github.com/titoBouzout/SideBarEnhancements) (Sublime 3 only, [Install on ST2](https://github.com/titoBouzout/SideBarEnhancements/issues/172))
- [ChangeQuotes](https://github.com/colinta/SublimeChangeQuotes) 
- [Gitgutter](https://github.com/jisaacks/GitGutter)
- [BracketHighlighter](https://github.com/facelessuser/BracketHighlighter)

> Want to create yours?    
> Plugins are open source, written in Python.
  

You should **never** work without syntaxic coloration!

--
## Extra: Usefull terminal aliases 1/2

Working with Heroku in multiple environment?

Add to your `~/code/dotfiles/aliases`

```
dev() {
  nocorrect heroku $* --app <APPNAME>-dev
}

prod() {
  nocorrect heroku $* --app <APPNAME>
}
```

And set your git remotes to those:

```
$ git remote -v
> origin  git@github.com:<REPONAME>/<APPNAME>.git
> dev git@heroku.com:<APPNAME>-dev.git
> prod  git@heroku.com:<APPNAME>.git
```

--
## Extra: Usefull terminal aliases 2/2
Then you can use in the terminal: 
```
git push dev master
dev run rake db:migrate
git push prod master
prod run rake db:migrate # <=> heroku run rake db:migrate --app <APPNAME>
prod run logs --tail # <=> heroku run logs --tail --app <APPNAME>
```
--
## Enjoy Coding with Sublime

You can practice by downloading this [file](practice.html)    
and apply the following changes:

- Correctly indent the file
- Change dates 2013 to 2014
- Add `target="_blank"` to every `<a>` tag