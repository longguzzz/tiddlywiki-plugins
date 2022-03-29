## tiddlywiki-plugins
### TagViewModifier
下载后拖拽到tiddlywiki中，会提示导入。

为了减少core的修改，本插件把TagViewModifier当作一个tiddler上可配置的部件，而不是修改原有的tiddler tag部分。

所以，安装后还需要如下操作：
1. 通过搜索打开shadow tiddler  `$:/core/ui/ViewTemplate/tags`, 为其添加标签`$:/longguzzz/ExcludeViewTemplate`, 这样就会在tiddler中排除原有的tag。
2. 继续点击shadow tiddler `$:/core/ui/ViewTemplate/tags` 的 `$:/tags/ViewTemplate` 标签，将 `$:/plugins/longguzzz/TagViewModifier/TagViewAndEdit` 拖拽至 `$:/core/ui/ViewTemplate/tags` 上方，这样就可以与原来的tag显示在同一个位置。
