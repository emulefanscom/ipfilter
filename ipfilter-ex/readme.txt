IPFilter v148 eMuleFans (2011-01-02)
by http://emulefans.com/news/plugin/ipfilter/ host on http://code.google.com/p/ipfilter-emule/

It is modified from Meuh6879's IPFilter v148 (2010-12-29), zmhleo's version and tetris's list. Level 0[EX] is used for some very bad IP. See or2ex.diff in SVN for the changing from Meuh6879's IPFilter. Thx Meuh6879, R3Qu13M, zmhleo and tetris.

====
IPFilter v148 eMuleFans修改版 (2011-01-02)
制作 http://emulefans.com/news/plugin/ipfilter/ 存于 http://code.google.com/p/ipfilter-emule/

在Meuh6879的IPFilter v148 (2010-12-29) （http://forum.emule-project.net/index.php?showtopic=19247）基础上，添加了之前本人所列举的迅雷离线下载服务器IP（http://emulefans.com/xunlei-server-ip-100802/）、zmhleo列举的疯狂检档IP（http://zmhleo.ys168.com/）、tetris等人的迅雷和QQ离线下载服务器IP（http://www.ied2k.com/forum/topic-23050.html），去除了肯定的特别是对服务器IP的误杀，不确定的服务器IP加了过滤级别，做了一些小修改。过滤级别0[EX]用于非常不良的IP。向Meuh6879、R3Qu13M、zmhleo、tetris等人致谢。相对于Meuh6879的IPFilter做的修改在SVN中的or2ex.diff（http://ipfilter-emule.googlecode.com/svn/trunk/ipfilter-ex/or2ex.diff）文件里。修改的详细说明在readme.txt（http://ipfilter-emule.googlecode.com/svn/trunk/ipfilter-ex/readme.txt）文件里。

====
使用方法

把解压出来的文件拷贝到eMule目录下的config目录里，然后启动eMule，进入选项的“安全”选项卡，把“过滤级别”设为95（建议），同时选中“服务器也被过滤”。

IPFilter eMuleFans修改版的长期维护更新地址，您可以添加至自动更新中（http://emulefans.com/plugin-auto-update-url/）：
http://sn.im/ipfilter.dat

====
详细说明

相对于Meuh6879做的修改差异请查看or2ex.diff（http://ipfilter-emule.googlecode.com/svn/trunk/ipfilter-ex/or2ex.diff）。这里是一些具体的说明：

剔除：

普通IP误杀：
60.255.0.0      - 60.255.255.255  , SiChuan Broadcasting & TV Net Co.,LTD
195.229.0.0     - 195.230.31.255  , Emirates Telecommunications Corporation, Proxy, City Heart Cafe
202.103.192.0   - 202.103.255.255 , [RT]CHINANET Guangxi pro, [L1]Nanning, NO.160 info, Power suppl, [L2]Nanning, Guangxi ban, [L1]Nanni
202.106.175.128 - 202.106.176.255 , [L1]Information & Communication Department
211.148.160.0   - 211.148.191.255 , TIANJIN BROADCAST &TV NETWORK CO., LTD（天津数字电视宽带服务）
211.245.230.0   - 211.245.252.255 , Thrunet Co., Ltd （THRUNET）（韩国的 ISP: SK Broadband）
218.98.0.0      - 218.98.223.255  , Shandong Beelink Information Technology Co., Ltd（山东百灵宽带）
219.84.0.0      - 219.85.255.255  , [L3]Sony Network Taiwan, [L1]Sony Network Taiwan, [DS][DShield top10] Unkn
219.106.224.0   - 219.106.255.255 , SONY Corporation（bit-drive）
219.139.192.0   - 219.140.255.255 , Chinanet network in Wuhan city Hubei province, Tor, Proxy（中国宽带互联网湖北省武汉市网络）
221.129.0.0     - 221.129.255.255 , [L1]TIANJIN BROADCAST & TV network Co., Ltd（天津数字电视宽带服务）
222.88.0.0      - 222.89.255.255  , CHINANET henan province network, LUOYANG AGRICULTURE BANK, SHANGQIU MINQUANG（中国宽带互联网河南省网络）
59.60.0.0       - 59.60.63.255    , [RT]CHINANET fujian prov, [L1]CHINANET|Anti-p2p, [FK]
61.128.0.0      - 61.129.255.255  , [L2] CNINFONET Backbone, [RT]Data Communication D, [L2] CNINFONET Xingjiang, [L1] Dushanzi Governmen
61.142.111.0    - 61.142.111.255  , [L1]CHINANET|Anti-p2p, [RT]CHINANET Guangdong p
61.234.99.0     - 61.234.99.255   , Jiangmen Broadcasting & TV Network Co.,Ltd
117.72.0.0      - 117.73.255.255  , Beijing Founder Broadband Network Technology Co.,Ltd
121.4.0.0       - 121.5.255.255   , Beijing Founder Broadband Network Technology Co.,Ltd
202.131.48.0    - 202.131.63.255  , Eastchina Broadcasting network Co.,Ltd
210.12.226.0    - 210.12.226.255  , Beijing Haidian Broadcasting & TV Network Co.,Ltd
211.156.128.0   - 211.156.159.255 , China Broadcasting TV Net
219.232.48.0    - 219.232.63.255  , Beijing Founder Broadband Network Technology Co.,Ltd

服务器误杀：
80.237.156.72   - 80.237.156.72   , bad ed2k server（free.usenet.nl 2）
87.230.0.0      - 87.230.127.255  , 120 , [RT]Hosteurope GmbH, [L2]Tor.Creo, [L2]Tor.tor4ccc, [L2]Tor.n0trace, [L1]www.heads-ltd.de, [L1]www.U
（www.UseNeXT.to）
88.191.81.111   - 88.191.81.111   ,  92 , [FK]Peer1-20101229
88.191.228.66   - 88.191.228.66   ,  92 , [FK]Peer2-20101229

==
更改与添加：


(ef)为eMuleFans所作更改：
Sharing Kingdom系列和freesxbay.com（88.80.28.48）服务器是否为伪造/钓鱼服务器尚有极大争议，Meuh6879 IPFilter中已将这些IP中的大部分列入110或120，剩下的一些我们也将它们IP的过滤级别加至100[L2]。不建议使用这些服务器，请考虑从服务器列表中删除它们，但也不一定需要过滤它们的IP。eMule IPFilter设置为95（标准）时候不过滤。
83.233.30.55    - 83.233.30.55    , 100 , [L2](ef)www.StormSex.net
83.233.30.126   - 83.233.30.128   , 100 , [L2](ef)www.StormSex.net


(LEO AbuseReQ)为自zmhleo版本增加的“疯狂检档IP”，加入级别60[EX]。
(XunleiOffline)和(QQOffline)为eMuleFans所作更改，为迅雷和QQ离线下载服务器，加入级别60[EX]。
58.61.39.209    - 58.61.39.255    ,   0 , [EX](XunleiOffline)
58.61.152.69    - 58.61.152.69    ,   0 , [EX](XunleiOffline)
58.251.57.66    - 58.251.57.125   ,   0 , [EX](XunleiOffline)
58.251.57.162   - 58.251.57.174   ,   0 , [EX](XunleiOffline)
58.251.59.4     - 58.251.59.6     ,   0 , [EX](XunleiOffline)
58.252.209.2    - 58.252.209.31   ,   0 , [EX](XunleiOffline)
58.254.134.201  - 58.254.134.253  ,   0 , [EX](XunleiOffline)
58.255.249.130  - 58.255.249.165  ,   0 , [EX](XunleiOffline)
58.255.253.130  - 58.255.253.156  ,   0 , [EX](XunleiOffline)
60.18.146.201   - 60.18.146.219   ,   0 , [EX](XunleiOffline)
60.18.147.194   - 60.18.147.211   ,   0 , [EX](XunleiOffline)
60.19.64.35     - 60.19.64.62     ,   0 , [EX](XunleiOffline)
60.21.219.66    - 60.21.219.108   ,   0 , [EX](XunleiOffline)
60.214.64.131   - 60.214.64.198   ,   0 , [EX](XunleiOffline)
60.221.254.158  - 60.221.254.200  ,   0 , [EX](XunleiOffline)
60.221.254.221  - 60.221.254.253  ,   0 , [EX](XunleiOffline)
61.54.12.130    - 61.54.12.151    ,   0 , [EX](XunleiOffline)
61.137.191.66   - 61.137.191.94   ,   0 , [EX](XunleiOffline)
61.147.76.2     - 61.147.76.93    ,   0 , [EX](XunleiOffline)
61.183.55.211   - 61.183.55.227   ,   0 , [EX](XunleiOffline)
61.235.71.73    - 61.235.71.73    ,   0 , [EX](XunleiOffline)
111.161.24.2    - 111.161.24.28   ,   0 , [EX](XunleiOffline)
116.55.230.131  - 116.55.230.211  ,   0 , [EX](XunleiOffline)
118.122.36.130  - 118.122.36.185  ,   0 , [EX](XunleiOffline)
118.122.87.18   - 118.122.87.23   ,   0 , [EX](XunleiOffline)
119.120.94.51   - 119.120.94.70   ,   0 , [EX](XunleiOffline)
119.120.94.130  - 119.120.94.228  ,   0 , [EX](XunleiOffline)
119.147.41.141  - 119.147.41.152  ,   0 , [EX](XunleiOffline)
119.178.12.2    - 119.178.12.23   ,   0 , [EX](XunleiOffline)
119.188.12.23   - 119.188.12.59   ,   0 , [EX](XunleiOffline)
121.9.209.3     - 121.9.209.18    ,   0 , [EX](XunleiOffline)
121.9.209.131   - 121.9.209.191   ,   0 , [EX](XunleiOffline)
121.9.246.2     - 121.9.246.39    ,   0 , [EX](XunleiOffline)
121.10.24.65    - 121.10.24.75    ,   0 , [EX](XunleiOffline)
121.10.120.136  - 121.10.120.164  ,   0 , [EX](XunleiOffline)
121.10.120.179  - 121.10.120.179  ,   0 , [EX](XunleiOffline)
121.10.120.235  - 121.10.120.241  ,   0 , [EX](XunleiOffline)
121.10.137.25   - 121.10.137.59   ,   0 , [EX](XunleiOffline)
121.10.137.131  - 121.10.137.140  ,   0 , [EX](XunleiOffline)
121.14.82.2     - 121.14.82.50    ,   0 , [EX](XunleiOffline)
121.14.82.130   - 121.14.82.157   ,   0 , [EX](XunleiOffline)
121.30.203.180  - 121.30.203.180  ,   0 , [EX](LEO AbuseReQ)CNCGROUP China169 Backbone datong shanxi
122.141.227.130 - 122.141.227.161 ,   0 , [EX](XunleiOffline)
122.228.241.2   - 122.228.241.46  ,   0 , [EX](XunleiOffline)
123.129.242.131 - 123.129.242.255 ,   0 , [EX](XunleiOffline)
124.115.1.0     - 124.115.2.255   ,   0 , [EX](QQOffline)
124.126.0.0     - 124.127.255.255 ,   0 , [EX](LEO AbuseReQ)Research Institution of Telecom
124.232.148.131 - 124.232.148.200 ,   0 , [EX](XunleiOffline)
125.39.72.11    - 125.39.72.208   ,   0 , [EX](XunleiOffline)
125.39.148.88   - 125.39.148.89   ,   0 , [EX](XunleiOffline)
125.39.149.2    - 125.39.149.100  ,   0 , [EX](XunleiOffline)
125.39.150.2    - 125.39.150.31   ,   0 , [EX](XunleiOffline)
125.46.42.130   - 125.46.42.130   ,   0 , [EX](XunleiOffline)
125.46.42.143   - 125.46.42.153   ,   0 , [EX](XunleiOffline)
125.221.46.131  - 125.221.46.138  ,   0 , [EX](XunleiOffline)
202.108.211.141 - 202.108.211.155 ,   0 , [EX](LEO AbuseReQ)Beijing Netparent Information Technology Co.Ltd
211.98.169.226  - 211.98.169.233  ,   0 , [EX](XunleiOffline)
211.137.100.86  - 211.137.100.87  ,   0 , [EX](XunleiOffline)
211.162.73.113  - 211.162.73.113  ,   0 , [EX](XunleiOffline)
218.6.13.101    - 218.6.13.124    ,   0 , [EX](XunleiOffline)
218.21.68.2     - 218.21.68.9     ,   0 , [EX](XunleiOffline)
218.59.144.2    - 218.59.144.13   ,   0 , [EX](XunleiOffline)
218.59.144.34   - 218.59.144.62   ,   0 , [EX](XunleiOffline)
218.75.172.139  - 218.75.172.139  ,   0 , [EX](XunleiOffline)
218.75.172.156  - 218.75.172.158  ,   0 , [EX](XunleiOffline)
219.129.83.2    - 219.129.83.31   ,   0 , [EX](XunleiOffline)
219.134.132.39  - 219.134.132.39  ,   0 , [EX](XunleiOffline)
219.134.132.56  - 219.134.132.57  ,   0 , [EX](XunleiOffline)
219.134.132.80  - 219.134.132.80  ,   0 , [EX](XunleiOffline)
219.141.210.160 - 219.141.210.179 ,   0 , [EX](LEO AbuseReQ)CCIDConsulting CNNIC beijing
219.143.87.173  - 219.143.87.173  ,   0 , [EX](LEO AbuseReQ)China Networks Inter-Exchange beijing
219.143.88.8    - 219.143.88.8    ,   0 , [EX](LEO AbuseReQ)China Networks Inter-Exchange beijing
219.143.95.204  - 219.143.95.204  ,   0 , [EX](LEO AbuseReQ)China Networks Inter-Exchange beijing
220.113.9.85    - 220.113.9.85    ,   0 , [EX](XunleiOffline)
220.249.103.131 - 220.249.103.138 ,   0 , [EX](XunleiOffline)
221.4.246.66    - 221.4.246.111   ,   0 , [EX](XunleiOffline)
221.5.8.25      - 221.5.8.41      ,   0 , [EX](XunleiOffline)
221.5.8.111     - 221.5.8.122     ,   0 , [EX](XunleiOffline)
221.203.179.3   - 221.203.179.21  ,   0 , [EX](XunleiOffline)
221.238.25.109  - 221.238.25.109  ,   0 , [EX](XunleiOffline)
222.70.180.108  - 222.70.180.108  ,   0 , [EX](LEO AbuseReQ)China Telecom (Group) Shanghai
222.141.53.2    - 222.141.53.74   ,   0 , [EX](XunleiOffline)