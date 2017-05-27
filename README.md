# gen-Report-from-svn
generate weekly report from svn submit
Usage:

# command withou any parameter, will show usage
```sh
$ processsvn
usage:
/-path-to-/processsvn week
/-path-to-/processsvn today
/-path-to-/processsvn week blame
/-path-to-/processsvn today blame
/-path-to-/processsvn today username
/-path-to-/processsvn week username
/-path-to-/processsvn today username blame
/-path-to-/processsvn week username blame
```

# command with today as parameter

```sh
$ processsvn today

user1: 本日(2017-05-27)开发了：
2017-05-27:
        r1306: xxxxxxxxxxxxxxxxxxxxxxxx
        r1303: xxxxxxxxxxxxxxxxxxxxxxxxx
        r1302: xxxxxxxxxxxxxxxxxxxxxxxxx
```

# command with week as parameter 
```sh
user1 本周(2017-05-22 - 2017-05-28)开发了:
2017-05-27:
	r1309: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1308: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1307: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1305: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1304: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1301: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
2017-05-26:
	r1299: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1298: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1294: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1290: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1287: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1275: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1272: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1271: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1270: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
2017-05-25:
	r1269: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1268: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1264: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1262: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1260: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1254: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1250: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1246: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1245: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1244: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
2017-05-24:
	r1238: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1235: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1231: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1230: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1229: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1217: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1216: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
2017-05-23:
	r1210: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1209: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1208: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1200: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1196: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1191: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
2017-05-22:
	r1188: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1187: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1185: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1181: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1180: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1179: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1177: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1174: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx


user2 本周(2017-05-22 - 2017-05-28)开发了:
2017-05-27:
	r1306: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1303: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1302: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
2017-05-26:
	r1297: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1296: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1295: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1293: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1292: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1291: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1289: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1288: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1286: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1285: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1284: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1283: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1282: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1281: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1280: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1279: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1278: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1276: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1274: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1273: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
2017-05-25:
	r1267: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1265: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1263: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1261: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1259: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1258: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1257: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1256: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1255: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1251: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1249: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1248: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1247: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1243: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1242: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1241: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1240: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
2017-05-24:
	r1237: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1236: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1234: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1233: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1232: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1228: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1227: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1226: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1225: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1224: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1222: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1221: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1220: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1218: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1215: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1214: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1213: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1212: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
2017-05-23:
	r1207: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1206: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1205: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1204: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1203: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1202: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1201: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1198: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1197: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1195: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1194: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1193: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1192: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1190: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
2017-05-22:
	r1186: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1184: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1183: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1182: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1178: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1176: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1175: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
	r1173: xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx


```


# command with today or week as first parameter, and userName as second parameter, will output the work done by this user only, for example,

```sh
$ processsvn today user1user1
user1: 本日(2017-05-27)开发了：
2017-05-27:
        r1306: xxxxxxxxxxxxxxxxxxxxxxx
        r1303: xxxxxxxxxxxxxxxxxxxxxxx
        r1302: xxxxxxxxxxxxxxxxxxxxxxx
```

# command with blame as parameter, will calculate the lines of codes which user has developed
```sh
 $ processsvn today user1 blame
Skipping binary file (use --force to treat as text): 'Application/README.md'
Skipping binary file (use --force to treat as text): 'Public/README.md'
user1: 本日(2017-05-27)开发了：
2017-05-27:
        r1306: xxxxxxxxxxxxxxxxxxx
        r1303: xxxxxxxxxxxxxxxxxxxxxxx
        r1302: xxxxxxxxxxxxxxxxxxxx
截至本日(2017-05-27)共开发了 13094 行代码。

```

# there's some config
1. protected $skipExt = ['png', 'jpg', 'doc', 'docx', 'pdf', 'mp4', 'gif', 'swf' ];
>* this control's file with extensions in the array will be ignored

2. protected $skipDirs = ['.', '..', 'Runtime', '.svn', '.git', 'images', 'ThinkPHP', 'lib'];
>* this control's the directory will be ignored.

3. protected $workingDirs = ['Application', 'Public'];
>* this control's the directory will be searched

4. protected $lang = 'zh';
>* $lang can either be 'zh' which means it will output Chinese, or 'en' which means it will output English

