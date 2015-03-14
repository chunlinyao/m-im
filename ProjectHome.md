<table>
<tr>
<td width='50%' valign='top'>
<h1>Welcome to the project page for m-im!</h1>

This project was started by chunlinyao to provide a light-weight J2ME application for connecting to GoogleTalk (GTalk), using older mobile phones like Nokia S40.<br>
<br>
Mark was added to the project in July 2009, and has been actively updating the code to add some new features. Mark is testing and developing for S60 Symbian, but wherever possible S40 will be fully supported!<br>
<br>
Version 1.3.1 of m-im has the following features:<br>
<br>
<ul><li>Connect to <code>GoogleTalk</code> or ANY XMPP / Jabber compliant service<br>
</li><li>Sound and/or Vibrate notifications for new messages<br>
</li><li>Multiple profiles (connect to one account only at a time)<br>
</li><li>Chat via GPRS, EDGE, 3G and 3.5G (HSDPA) and WIFI connections (and more?)<br>
</li><li>XMPP Keepalive - I have left m-im connected for over 24 hours without problems! (Mark)<br>
</li><li>English and Chinese user interface, other translations can be added as required!<br>
</li><li>Minimise (run in background) support for S60 phones</li></ul>

Grab the <a href='http://code.google.com/p/m-im/downloads/list?q=label:Latest'>Latest Version</a> from the downloads section and install it on your phone.<br>
<br>
See the ChangeLog for details about each release and history<br>
<br>
</td>

<td width='50%' valign='top'>
(<font color='red'>注：中文介绍已经较长时间未更新</font>)<br>
这个工程是把MGtalk和jxa结合起来了。<br>
<br>
<h3>简介</h3>
前一段时间我的MGtalk不能访问Gtalk了，所以想自己动手修改一下，发现实在搞不懂他的<code>XmlNode</code>和<code>NetworkDispatcher</code>部分，所以想把XMPP协议处理部分换掉，找到了Jxa，发现他的XMPP实现还是比较容易看懂的。因为使用的两个工程都是GPL的，所以这个工程也是用GPL v2发布。（并不代表本人支持GPL :-| ）<br>
<br>
<h3>状态</h3>
目前把两个项目结合后，添加了Google的<code>SharedStatus</code>支持。取消了Gmail通知（觉得浪费带宽），认证使用X-GOOGLE-TOKEN和PLAIN两种。<br>
有一些BUG，可以正常使用。<br>
<br>
<h3>下一步</h3>
下一步也许不会发生。如果发生的话可能是以下几个；<br>
<del>整理Jxa的代码。发送信息采用一个单独的线程；（生产者消费者）</del>

重开一个分支：<br>
界面不用MGTalk的代码，用非GPL的替换掉；<br>
<del>XMPP不用Jxa,用kxml自己实现（kxml是BSD协议的）；</del>
1.5.0已经重新用kxml实现XMPP协议部分。<br>
<br>
如果你对这些改造感兴趣，希望你加入。<br>
<br>
</td>
</tr>
</table>