# Visual Studio Code `Journey`

- [Setup vscode command line access](#setup-vscode-access-from-command-line)

- [Export your vscode exrtensions list](#setup-vscode-access-from-command-line)

- [Extensions that i may or may not use :stuck_out_tongue_winking_eye:](extensions.md)

### Setup VSCode command line access

You may want to access visual studio code from command line (`terminal`).

Simple... just press 

<kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>p</kbd>

type `shell` and select ( Shell Command: Install 'code' command in PATH ).

### Export your vscode exrtensions list

After [adding visual studio code to PATH](#setup-vscode-command-line-access), you can see the list of the installed extensions by running.

```
code --list-extensions

```

And you can generate the code for importing ( installing ) these extensions automatically as described by [Benny](https://stackoverflow.com/users/2243665/benny) in his [answer](https://stackoverflow.com/a/49398449) on stackoverflow.

1. On machine A : Depending on your OS, copy the output of the this command 

Unix:
```
code --list-extensions | xargs -L 1 echo code --install-extension
```
Windows (PowerShell):
```
code --list-extensions | % { "code --install-extension $_" }
```

Sample output

```
code --install-extension extension-a
code --install-extension extension-b
...
```

2. On machine B : Paste the output in your shell.
