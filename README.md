# TumblThree 简体中文

这儿是[TumblThree](https://github.com/TumblThreeApp/TumblThree)的英语和简体中文的源文件。

This is Emphasia's Simplified Chinese translation for [TumblThree](https://github.com/TumblThreeApp/TumblThree).

**为更好地开发，TumblThree已迁移，请查看其新主页：[TumblThreeApp/TumblThree](https://github.com/TumblThreeApp/TumblThree)**

- 原作者repo：[johanneszab/TumblThree](https://github.com/johanneszab/TumblThree)
- 现项目repo：[TumblThreeApp/TumblThree](https://github.com/TumblThreeApp/TumblThree)
- 程序BUG或建议：
  - 向开发者提*（建议英语）*：https://github.com/TumblThreeApp/TumblThree/issues
  - 向我提*（中英皆可）*：https://github.com/Emphasia/TumblThree-zh/issues
  - 注意：在国内的网络环境下，**设定用于下载的代理**可能是必须的，这并不是TumblThree的BUG。

## 下载 Download

👉 https://github.com/Emphasia/TumblThree-zh/releases

> 因语言文件越来越臃肿，作者已将主程序和语言文件分别发布。
>
> 此处的发布只是把作者发布的两部分整合后保留中英得到的。
>
> ~~同步的版本因新功能的增加可能会有未翻译和错误的情况，而完全翻译的版本一般会晚一个版本。~~
>
> 因个人原因，此处的发布无法及时更新，请查看[项目releases](https://github.com/TumblThreeApp/TumblThree/releases)。

TumblThree作者的最新版本、别的版本及更新历史：https://github.com/TumblThreeApp/TumblThree/releases

## 新手入门 Getting Started

默认的设置应该已经能满足大多数用户的需求，你只需要再选定一个**下载目录**和你**要下载的帖子类型** 。对此，你可能想要在`设置`中更改：

- `下载` -> `下载目录`：指定下载的文件的存放位置。默认在程序根目录下。
- `博客` 中的设置作为新添加的博客的默认设置*（仅对新添加的博客有效）*

  要改变单独某个博客的下载，在`主界面`选中该博客，转到右侧`详细`标签页并更改设置。同时更改多个博客的下载设置请使用`Shift + 左键`或`Ctrl + A`全选。
- 注意：你可能总是想要选中启用：
  - _下载转发的帖_：下载博主转发的帖子而不只是其原创的帖子 。

当你感觉**下载速度不理想时**可能想更改的设置：

- `下载` -> HTTP代理：设定用于下载的代理。**注意：在国内的网络环境下，这可能是必须的。**（也可以考虑修改hosts😏）
- `下载` -> 并发连接数：设定用于下载帖子的连接的数目。该数目将被所有当前正在下载的博客共用。注意：如果你只下载视频帖子，你也许想要减少并行连接数至8或更低，具体取决于你的网络状况。否则你可能会因为tumblr服务器频繁的关闭连接（同时打开了太多连接）而得到不完整的文件。对小文件（如图片）这没啥影响。
- `下载` -> 并发视频数：设定用于下载视频的连接的数目。该数目将被所有当前正在下载的博客共用。注意：当同时打开太多连接时，tumblr视频服务器(vt.tumblr.com)会频繁的关闭连接，从而导致得到不完整的文件。因此，设置此选项以供单独设定与其最大连接数。
- `下载` -> 并发博客数：同时处理的博客数量。

一般情况下你不需要改变其他的连接设置。特别的，除非你明确知道其作用否则不要去更改的：

- `下载` -> 限制Tumblr-API连接数：保持选中启用且不要改变对应的值（默认*90连接数每60秒*）。如果你执意更改，你可能会得到*博客离线*或*下载不全*等问题。

## 使用指南 Usage

- 下载并解压 `.zip` 文件，运行 `TumblThree.exe`。
- 复制想要备份或下载的tumblr博客`URL`(blogname.tumblr.com)到底部的文本框（或使用剪贴板监视功能自动添加）后，点击右边的 `添加博客`。
- 先将要处理的博客`添加到队列`，然后单击`开始`来开始下载（爬取），程序将自动检查队列中的博客并处理，直到你按下`停止` 。当然，你可以也可以先开始再向队列中添加博客。
- 队列中博客左边的蓝条表明这个博客正在下载，左边的博客管理器也表明了各个博客的状态（红色为离线，绿色为下载中，紫色为等待）。
- 你可在`设置`中设置并行的博客数目，下载目录和指定图片分辨率，或自动下载的时间。
- 在`详细`标签页你可以查看博客的数据和设置下载选项（要下载的帖子种类、特定标签、时间段等）。
  - 下载带特定标签的帖子：
    1. 添加该博客
    2. 在`详细`标签页`标签`文本框输入以‘,’分隔的标签（E.g. _great big car,bears_）
    3. 将该博客添加到队列并下载
  - 下载密码保护博客的帖子：
    1. 添加该博客
    2. 在`详细`标签页`密码`文本框输入该博客的密码
    3. 将该博客添加到队列并下载
  - 下载隐藏博客（需要登录才可以浏览）的帖子：
    1. 到`设置` -> `连接`标签页填入 *登录邮箱与密码* ，单击`授权`登录tumblr，登陆成功后标签页将显示你的邮箱地址
    2. 添加该博客
    3. 将该博客添加到队列并下载
  - 下载某用户喜欢过的图片和视频：
    1. 到`设置` -> `连接`标签页填入 *登录邮箱与密码* ，单击`授权`登录tumblr，登陆成功后标签页将显示你的邮箱地址
    2. 添加该博客（包括liked/by字符串 e.g. https://www.tumblr.com/liked/by/wallpaperfx/）
    3. 将该博客添加到队列并下载

    下载您 **自己的“喜欢”** 时，请确认您已经在您的博客设置 (https://www.tumblr.com/settings/blog/ *你的博客名*) 中（临时地）启用以下选项：
    + `Likes` -> Share posts you like (使 “喜欢”页 公开)
    + `Visibility` -> _blog_ is explicit (使 NSFW “喜欢” 可见/可下载)
  - 下载tumblr搜索结果中的图片和视频：
    1. 到`设置` -> `连接`标签页填入 *登录邮箱与密码* ，单击`授权`登录tumblr，登陆成功后标签页将显示你的邮箱地址
    2. 添加该博客（包括以‘+’分隔的关键词 e.g.  https://www.tumblr.com/search/my+keyword）
    3. 将该博客添加到队列并下载
  - 下载tumblr标签搜索结果中的图片和视频：
    1. 到`设置` -> `连接`标签页填入 *登录邮箱与密码* ，单击`授权`登录tumblr，登陆成功后标签页将显示你的邮箱地址
    2. 添加该博客（包括以‘+’分隔的标签 e.g.  https://www.tumblr.com/tagged/my+special+tags）
    3. 将该博客添加到队列并下载


### 进阶使用 Further Insights

- 快捷键
  - 双击博客可将其添加到队列
  - 从左侧博客管理器直接拖拽到队列来添加
  - `空格` - 开始
  - `Ctrl + 空格` - 暂停
  - `Shift + 空格` - 停止
  - `Del` - 从队列移除
  - `Shift + Del` - 从博客管理器移除
  - `Ctrl + Shift + G` - 开始垃圾回收

- 保存的文件

  注意：以下文件都以json格式保存于 _%LOCALAPPDATA%_ （C:\\Users\\*用户名*\\AppData\\Local\\）

  - 登陆成功后，用户名邮箱地址与密码不保存，但cookies将生成并保存于_%LOCALAPPDATA%\TumblThree_
  - 设置文件Settings.json保存在 _%LOCALAPPDATA%\TumblThree_
  - 你可以使用 *便携模式* (设置->全局) 将设置文件保存在程序根目录
  - 对每个博客，在下载目录（默认在程序根目录下的 _.\\Blogs\\_）下有一个以博客名命名的 索引(*Index*)文件夹 中有 数据库(序列化类) 文件。其中储存了博客URL、何时添加、哪些文件已被下载等信息。这使你能够移动已下载的文件到别的目录而不影响下载过程。

- 另有一些设置未在UI中显示，要查看或修改全部的设置可打开设置文件Settings.json。

  其中一些值得注意的可以进一步优化应用程序的设置：

  - BufferSize：设定下载时的缓存大小（为4KB的倍数，其默认值为512即大小为4KB*512=2MB）。增大其值会减少磁盘碎片因为文件将先在内存中积攒并一次性连块写入磁盘，但同时也会因此增加内存的使用量。
  - MaxNumberOfRetries：设定当服务器强制关闭连接时重试次数的上限。当同时打开太多与tumblr视频服务器(vt.tumblr.com)的连接时这可能会经常发生。当此上限被耗尽时，文件就会下载不完整（下一次下载时会恢复继续下载）。
  - TumblrHosts：包含一系列在下载原始(\_raw)图片时用来尝试的服务器(hosts)。如果所有的服务器都不包含原始(\_raw)版本，将会继续尝试较低一级的分辨率(1028)。

## 功能 Features

* 多线程下载
* 监视剪贴板中URL(*blogname.tumblr.com*)并自动添加博客到列表
* 图片和视频可预览
* 可自定义下载目录
* 可导出下载地址而不实际下载
* 下载队列可自动保存
* 下载队列可导出、清空和恢复
* 可设置指定（下载）分辨率
* 可跳过下载已在别的博客（当前已加载的）下载过的文件
* 可用便携模式
* 可用HTTP代理（调用系统代理即IE）
* 可限制带宽和线程
* 可设置自动下载
* 使用SSL而不是不安全的HTTP连接
* 任务栏图标和快捷键绑定

### 博客备份或下载 Blog backup/download

* 可下载图片、视频、文本、音频、引用、对话、链接和回复贴
* ~~可下载图片、视频、音频的元数据~~ [（截至2018.8.10，Tumblr元数据已无法获取）](https://github.com/johanneszab/TumblThree/issues/261)
* 可下载内嵌的图片和视频
* 可下载safe-mode、密码保护或隐藏以及NSFW的博客
* 可下载外链 Imgur, Gfycat, webmshare, Mixtape, lolisafe, Uguu, Catbox, SafeMoe 的帖子
* 可仅下载原创帖而跳过转发帖
* 可仅下载带标签（或指定标签）的帖子
* 可下载特定页数或时间段内的帖子而不是整个博客
* 可下载某用户喜欢❤过的图片和视频 (e.g. https://www.tumblr.com/liked/by/wallpaperfx/) (需要登录)
* 可下载tumblr搜索结果中的图片和视频 (e.g. http://www.tumblr.com/search/my+keywords)
* 可下载tumblr标签搜索结果中的图片和视频 (e.g. http://www.tumblr.com/tagged/my+keywords) (需要登录)


### 不足之处 Limitations

- Windows XP 已不支持
