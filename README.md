```
[Script]
http-response ^https?:\/\/(api|mapi)\.weibo\.(cn|com)\/2(\/groups\/timeline|\/statuses\/unread|\/statuses\/extend|\/comments\/build_comments|\/photo\/recommend_list|\/stories\/video_stream|\/statuses\/positives\/get|\/stories\/home_list|\/profile\/statuses|\/statuses\/friends\/timeline|\/service\/picfeed) script-path=https://raw.githubusercontent.com/yichahucha/surge/master/wb_ad.js,max-size=-1
http-response ^https?:\/\/(sdk|wb)app\.uve\.weibo\.com(\/interface\/sdk\/sdkad.php|\/wbapplua\/wbpullad.lua) script-path=https://raw.githubusercontent.com/yichahucha/surge/master/wb_launch.js

[MITM]
hostname = api.weibo.cn, mapi.weibo.com, *.uve.weibo.com
```
