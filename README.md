## tiddlywiki-plugins

### TagViewModifier
![image](https://user-images.githubusercontent.com/96779663/160603471-81e0552e-4210-4ec2-960e-905cc21ff069.png)

下载后拖拽到tiddlywiki中，会提示导入。

对tiddlywiki core中原有的ViewTemplate和EditTemplate中的tags部分进行了合并。为了减少core的修改，本插件把TagViewModifier当作一个tiddler上可配置的部件，而不是修改原有的tiddler tag部分。

所以，安装后还需要如下操作：
1. 通过搜索打开shadow tiddler  `$:/core/ui/ViewTemplate/tags`, 为其添加标签`$:/longguzzz/ExcludeViewTemplate`, 这样就会在tiddler中排除原有的tag。
2. 继续点击shadow tiddler `$:/core/ui/ViewTemplate/tags` 的 `$:/tags/ViewTemplate` 标签，将 `$:/plugins/longguzzz/TagViewModifier/TagViewAndEdit` 拖拽至 `$:/core/ui/ViewTemplate/tags` 上方，这样就可以与原来的tag显示在同一个位置。

### OpenForest
![image](https://user-images.githubusercontent.com/96779663/160603348-115b82d9-ad94-4cff-8402-26c44a1525ee.png)
1. 这个插件是在$:/plugins/sq/Stories的代码上加入了$:/plugins/ihm/tidgraph进行轻度魔改。
2. 使用这个插件不一定要添加$:/plugins/sq/Stories，但是必须添加$:/plugins/ihm/tidgraph。加了$:/plugins/sq/Stories的话，右侧栏也能有同样的效果
3. 要修改展示的深度，打开$:/plugins/longguzzz/OpenForest/ui/SideBar/Open，搜索maxdepth，修改引号里的数字就可以了。具体怎么用，参考插件$:/plugins/ihm/tidgraph

相关插件具体参见 https://giffmex.org/stroll/stroll.html，和 https://ihm4u.github.io/tw5plugs/
