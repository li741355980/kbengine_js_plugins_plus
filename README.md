# kbengine_js_plugins_plus
解决原kbengine js插件在win32平台下出现的分包问题（html5、win32、android、ios下测试通过）</br>
# 使用方法</br>
1.在jsList中加入此文件（位于"plugins/kbengine_js_plugins/kbengine.js"之后）</br></br>
2.在cc.game.onStart 中替代KBEngine.create 为 :</br>
KBEngine.init("127.0.0.1", 20013)</br>
也可替代为：</br>
var args = new KBEngine.KBEngineArgs();</br>
args.ip = "127.0.0.1";</br>
args.port = 20013;</br>
KBEngine.init(args);</br>
