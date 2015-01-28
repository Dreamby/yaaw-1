YAAW
====

你好，这里是由 KK 酱汉化的 YAAW~

这是一个用纯 HTML/CSS/Javascirpt 制造的 Aria2 客户端.

不需要后台或是服务器支持. 只需在浏览器中打开页面就能使用.

<br />

使用方法
-----
1. 开启 aria2 的 JSON-RPC 支持
> aria2c --enable-rpc --rpc-listen-all=true --rpc-allow-origin-all
>
> 警告: JSON-RPC 功能使用过程不会进行校验. 请确保地址不被泄露.

2. 使用浏览器打开 **index.html**.

3. 如果出现 "Internal server error" 错误，请在设置中修改 "JSON-RPC 回调地址".

技巧提示
----
* 所有设置都将被临时保存在浏览器中. **重启 Aria2 后需要重新应用设置.**
* 任务列表(含未完成任务) 将在 Aria2 重启后丢失. 使用 `--save-session=SOME/WHERE` 保存任务列表，并且使用 `--continue=true --input-file=SOME/WHERE` 参数载入任务列表.
* 使用 `$HOME/.aria2/aria2.conf` 保存您的设置.
* 获取 Aria2 的更多信息, 请访问 [Aria2 用户手册](http://aria2.sourceforge.net/manual/en/html/)

用到的组件：
----------
+ [Bootstrap](http://twitter.github.com/bootstrap/)
+ [mustache.js](https://github.com/janl/mustache.js)
+ [jQuery](http://jquery.com/)
+ [jQuery Storage](http://archive.plugins.jquery.com/project/html5Storage)
+ [JSON RPC 2.0 jQuery Plugin](https://github.com/datagraph/jquery-jsonrpc)

License
-------
yaaw is licensed under GNU Lesser General Public License.
You may get a copy of the GNU Lesser General Public License from http://www.gnu.org/licenses/lgpl.txt
