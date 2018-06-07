## 设置开发环境
### 普通的setting配置
* 设置smooth字体：`"workbench.fontAliasing": "antialiased"`
* 设置terminal的zsh：`"terminal.integrated.shell.osx": "/bin/zsh"`

### 通用快捷键设置
* 改变当前的窗口大小
```
{
  "key": "cmd+r",
  "command": "workbench.action.increaseViewSize"
},
{
  "key": "cmd+e",
  "command": "workbench.action.decreaseViewSize"
}
```

* 设置cmd+(=/-)时，只改变editor的文字大小
```
{
  "key": "cmd+numpad_add",
  "command": "editor.action.fontZoomIn"
},
{
  "key": "shift+cmd+=",
  "command": "editor.action.fontZoomIn"
},
{
  "key": "cmd+=",
  "command": "editor.action.fontZoomIn"
},
{
  "key": "cmd+numpad_subtract",
  "command": "editor.action.fontZoomOut"
},
{
  "key": "shift+cmd+-",
  "command": "editor.action.fontZoomOut"
},
{
  "key": "cmd+-",
  "command": "editor.action.fontZoomOut"
},
{
  "key": "cmd+numpad0",
  "command": "editor.action.fontZoomReset"
},
{
  "key": "cmd+0",
  "command": "editor.action.fontZoomReset"
}
```

* 设置在sidebar中添加文件和文件夹的快捷键
```
{
  "key": "cmd+n cmd+o",
  "command": "explorer.newFolder"
},
{
  "key": "cmd+n cmd+f",
  "command": "explorer.newFile"
}
```

### vim配置
* 安装`amVim`
* 配置特性：设置"editor.lineNumbers": "relative"后，可以使用 `n+k`：上移动到某一行，`n+j`：下移动到某一行

### 字符跳转配置
* 安装`metaGo`
* 配置快捷键
```
{
  "key": "cmd+;",
  "command": "metaGo.goto",
  "when": "editorTextFocus"
},
{
  "key": "alt+;",
  "command": "-metaGo.goto",
  "when": "editorTextFocus"
},
{
  "key": "shift+cmd+;",
  "command": "metaGo.selection",
  "when": "editorTextFocus"
},
{
  "key": "shift+alt+;",
  "command": "-metaGo.selection",
  "when": "editorTextFocus"
}
```

