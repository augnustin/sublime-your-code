![Sublime Text](/assets/logo-sublime-3.png)

# Sublime 
# your code

by [Augustin Riedinger](http://augustin-riedinger.fr)
--
## Access your code

#### Among the project

|                                    | ![Linux](/assets/linux-logo.png) | ![Mac](/assets/OS_X-Logo.png) |
|:----------------------------------:|:--------------------------------:|:---------------------:|
|     Access a file with filename    |            ![Ctrl](/assets/keyboard/ctrl.png) + ![P](/assets/keyboard/p.png)            |       ![Cmd](/assets/keyboard/cmd.png) + ![P](/assets/keyboard/p.png)       |
| Access a file with snippet of code |        ![Ctrl](/assets/keyboard/ctrl.png) + ![Shift](/assets/keyboard/shift.png) + ![F](/assets/keyboard/f.png)        |   ![Ctrl](/assets/keyboard/ctrl.png) + ![Shift](/assets/keyboard/shift.png) + ![F](/assets/keyboard/f.png)  |
|     Access a method definition     |               ![F12](/assets/keyboard/f12.png)              |                       |

--
## Access your code

#### Within the opened file
|                                    | ![Linux](/assets/linux-logo.png) | ![Mac](/assets/OS_X-Logo.png) |
|:----------------------------------:|:--------------------------------:|:-----------------------------:|
|     Access line number             | ![Ctrl](/assets/keyboard/ctrl.png) + ![G](/assets/keyboard/g.png) | ![Cmd](/assets/keyboard/cmd.png) + ![G](/assets/keyboard/g.png)       |
|     Access symbol                  |            ![Ctrl](/assets/keyboard/ctrl.png) + ![R](/assets/keyboard/r.png)            |       ![Cmd](/assets/keyboard/cmd.png) + ![R](/assets/keyboard/r.png)       |

--
## Move your code

|                   | ![Linux](/assets/linux-logo.png) |  ![Mac](/assets/OS_X-Logo.png) |
|:-----------------:|:--------------------------------:|:------------------------------:|
|  Duplicate a line |        ![Ctrl](/assets/keyboard/ctrl.png) + ![Shift](/assets/keyboard/shift.png) + ![D](/assets/keyboard/d.png)        |       ![Ctrl](/assets/keyboard/ctrl.png) + ![Shift](/assets/keyboard/shift.png) + ![D](/assets/keyboard/d.png)       |
| Move up/down line |  ![Ctrl](/assets/keyboard/ctrl.png) + ![Shift](/assets/keyboard/shift.png) + ![Up](/assets/keyboard/cursor-up.png)/![Down](/assets/keyboard/cursor-down.png)  | ![Ctrl](/assets/keyboard/ctrl.png) + ![Shift](/assets/keyboard/shift.png) + ![Up](/assets/keyboard/cursor-up.png)/![Down](/assets/keyboard/cursor-down.png) |
|  Move right/left  |          ![Tab](/assets/keyboard/tab.png)/![Shift](/assets/keyboard/shift.png)+![Tab](/assets/keyboard/tab.png)         |         ![Tab](/assets/keyboard/tab.png)/![Shift](/assets/keyboard/shift.png)+![Tab](/assets/keyboard/tab.png)        |
|   Comment/Uncomment a line  |        ![Ctrl](/assets/keyboard/ctrl.png) + ![Shift](/assets/keyboard/shift.png) + ![Slash](/assets/keyboard/keypad-slash.png)        |       ![Cmd](/assets/keyboard/cmd.png) + ![Slash](/assets/keyboard/keypad-slash.png)       |

> You barely never need multiple-line comments

--
## Multiple Edits

|                                | ![Linux](/assets/linux-logo.png) | ![Mac](/assets/OS_X-Logo.png) |
|:------------------------------:|:--------------------------------:|:-----------------------------:|
|     Create multiple cursor     |          ![Ctrl](/assets/keyboard/ctrl.png) + Click          |         ![Ctrl](/assets/keyboard/ctrl.png) + Click        |
|   Select multiple occurrences  |            ![Ctrl](/assets/keyboard/ctrl.png) + ![D](/assets/keyboard/d.png)            |           ![Ctrl](/assets/keyboard/ctrl.png) + ![D](/assets/keyboard/d.png)          |
| Break line in multiple cursors |            ![Ctrl](/assets/keyboard/ctrl.png) + ![L](/assets/keyboard/l.png)            |           ![Ctrl](/assets/keyboard/ctrl.png) + ![L](/assets/keyboard/l.png)          |
| Break line in multiple cursors |        ![Ctrl](/assets/keyboard/ctrl.png) + ![Shift](/assets/keyboard/shift.png) + ![L](/assets/keyboard/l.png)        |       ![Ctrl](/assets/keyboard/ctrl.png) + ![Shift](/assets/keyboard/shift.png) + ![L](/assets/keyboard/l.png)      |
|      Undo select operation     |            ![Ctrl](/assets/keyboard/ctrl.png) + ![U](/assets/keyboard/u.png)            |    ![Cmd](/assets/keyboard/cmd.png) + ![U](/assets/keyboard/u.png)                           |

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
[Add a goto method definition click shortcut](http://stackoverflow.com/questions/16235706/sublime-3-set-key-map-for-function-goto-definition)

--
## Usefull Plugins

Install [plugins](https://sublime.wbond.net/installation): ![Ctrl](/assets/keyboard/ctrl.png) + ![Shift](/assets/keyboard/shift.png) + ![P](/assets/keyboard/p.png) --> `Install Package`

- [Sidebar enhancement](https://github.com/titoBouzout/SideBarEnhancements) (Sublime 3 only)
- [ChangeQuotes](https://github.com/colinta/SublimeChangeQuotes) 
- [Gitgutter](https://github.com/jisaacks/GitGutter)
- [BracketHighlighter](https://github.com/facelessuser/BracketHighlighter)

> Want to create yours?    
> Plugins are open source, written in Python.
  

You should **never** work without syntaxic coloration!

--
## Extra: Usefull terminal aliases

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
> origin  git@github.com:copass/copass.git
> dev git@heroku.com:<APPNAME>-dev.git
> prod  git@heroku.com:<APPNAME>.git
```

--
Then you can use in the terminal: 
```
git push dev master
dev run rake db:migrate
git push prod master
prod run rake db:migrate # <=> heroku run rake db:migrate --app <APPNAME>
prod run logs --tail # <=> heroku run logs --tail --app <APPNAME>
```