# 同文小鹤音形方案使用说明

20201024超级更新，直接在Love Fly方案基础上，实现了自动和手动造词。将方案复制到用户文件夹部署后，选择Love Fly方案即可。

#注意：所有文件需全部复制才能实现效果，包括flypyzc方案。

<br\>

小鹤双拼音形自动造词输入方案：固定原码表词序，开启自动和手动造词，词序居后。

需先到小鹤音形官方网盘下载小鹤第三方Rime挂接版方案。

1. 复制到用户文件夹即可，重新部署后进入方案选单勾选~~Auto Fly~~ Love Fly方案。~~不影响小鹤自带方案，会出现一部分罕用单字打不出来，但是可以利用小鹤官方自带反查功能打出。~~
2. 自动造词最大词长设置为4，max_phrase_length: 4，可自行更改为更高值。若设置encode_commit_history: false，则屏蔽自动造词功能。
3. 用单引号 ' 启用语句流功能实现手动造词，造词时使用单引号 ' 分词。
4. flypyzc.extended.yaml 为用户词库，若含有编码，和系统词库重码时置顶。也可直接批量写入词条，会自动根据规则生成编码，和系统词库重码时居后（多音字的可能需要自行设定）。
5. trime.yaml中，将键o,p,k原有的符号改成了上划，长按改成了←，→和删词。取消了shift在打字时变成esc键，将esc功能改成了退格键上滑。退格键左滑为隐藏候选栏。

PS：（1）感谢鹤大的小鹤双拼音形输入法，给予日常输入带来的巨大便利。https://flypy.com/
    （2）谢谢omgredfog的五笔方案启发 https://github.com/omgredfog/98wubi
