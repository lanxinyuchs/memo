**需要转义的字符较多时**

sed 's!/bin/bash!/bin/csh!' /etc/passwd

**替换部分行中的匹配**

sed '2,3/old/new/' data.txt

**替换某一行**

sed '3c\

&gt;This is a change.' data.txt

**^开头 $结尾 d删除 a追加 i插入**

