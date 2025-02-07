# heroku搭建v2ray服务器

 fork！github项目：

* [v2hero](https://github.com/onplus/v2hero)

使用现成的[模板](https://heroku.com/deploy?template=https://github.com/onplus/heroku_go-getting-started)，默认的uuid有冲突所以需要更改

<!-- ![](https://ipfs.io/ipfs/QmYMotFhdsdFK2nbro8psM9DrfPuGfoR1UW6Wcfhyp8e9u?2.png) -->

![](https://raw.githubusercontent.com/hoodiearon/fq-book/master/docs/images/2018-05-16_073517.png)

使用[uuidgenerator](https://www.uuidgenerator.net/)刷新一次页面每次均生成不同uuid

<!-- ![](https://ipfs.io/ipfs/QmdosJDGsEi9aXg9J42BgaRdV4qrEE7BCRCh1HuxwVt2Uc?3.png) -->

![](https://raw.githubusercontent.com/hoodiearon/fq-book/master/docs/images/2018-05-16_073839.png)

复制uuid粘贴进入uuid填写空中并确定

<!-- ![](https://ipfs.io/ipfs/QmZ2jV6DEyoAaAQ45gAsfYZUnYnqjSfPpLqWhVYWGg4cL7?3.png) -->

![](https://raw.githubusercontent.com/hoodiearon/fq-book/master/docs/images/2018-05-16_080047.png)

授权登录[travis-ci](https://travis-ci.org/profile)中开启按钮并设置

<!-- ![](https://ipfs.io/ipfs/QmTvirGSXtuXiBJNjKBeUAQZqvZT4qy9YNVqTSX11BPQKj?0.png) -->

![](https://raw.githubusercontent.com/hoodiearon/fq-book/master/docs/images/2018-05-16_074407.png)

在`setting`选项中找到`Environment Variables`

<!-- ![](https://ipfs.io/ipfs/QmPXP33L7Pr9zRLykptoKcvviJuRypviVTLfmensgQxkBG?4.png) -->

![](https://raw.githubusercontent.com/hoodiearon/fq-book/master/docs/images/2018-05-16_080618.png)

环境变量相关参数

|name|value|
|:-:|:-:|
|HEROKU_APPNAME|heroku应用名称|
|HEROKU_EMAIL|注册heroku的邮箱|
|HEROKU_APIKEY|heroku的apikey| 

添加写入相应键值数据
<!-- ![](https://ipfs.io/ipfs/QmPGKFVeEbPb8x2hkTDnx4X1RwEWiV7FpsKZr22n6gpqyb?1.png) -->

![](https://raw.githubusercontent.com/hoodiearon/fq-book/master/docs/images/2018-05-16_081238.png)

关于`api key`的位置，点击头像选择`account setting`往下拉即可看到

<!-- ![](https://ipfs.io/ipfs/QmbricYnEEoG4sn3tCnqVidrHdcaioWjiPZbXgfjKBZUyd?1.png) -->

![](https://raw.githubusercontent.com/hoodiearon/fq-book/master/docs/images/2018-05-16_081848.png)

按步骤构建即可

<!-- ![](https://ipfs.io/ipfs/Qmc93xvtPjj3fFgfGPX9kppM8tr8LdBTgg4hniNe4sAKpg?0.png) -->

![](https://raw.githubusercontent.com/hoodiearon/fq-book/master/docs/images/2018-05-16_082146.png)

等待片刻，黄色变成绿色即可

<!-- ![](https://ipfs.io/ipfs/QmYko1LSWdnnAGFcuijvxP7WesjBuUU3eQ5XmMnSU45CMK?2.png) -->

![](https://raw.githubusercontent.com/hoodiearon/fq-book/master/docs/images/2018-05-16_082553.png)

在heroku的`more`选项中选择`Restart Dynos`并再次选择就行

<!-- ![](https://ipfs.io/ipfs/QmYkUkyuG6UzPrYBqSAdMR12VFoA5kyf1ANSWVvMG45QDo?0.png) -->

![](https://raw.githubusercontent.com/hoodiearon/fq-book/master/docs/images/2018-05-16_083502.png)

`view logs`确认启动成功

<!-- ![](https://ipfs.io/ipfs/QmRCMqygTFgB8HRsfUD5zyQH33tkE2RnExCGjrDP7RA3Bk?2.png) -->

![](https://raw.githubusercontent.com/hoodiearon/fq-book/master/docs/images/2018-05-16_083035.png)

以v2rayN为例

<!-- ![](https://ipfs.io/ipfs/QmbQQ2im8gdNKfLtQ6WPv1YTZ448EsRuLgP3hSSP8gpqqq?3.png) -->

![](https://raw.githubusercontent.com/hoodiearon/fq-book/master/docs/images/2018-05-16_090353.png)

填入相应的配置参数并确定，id就是你的uuid，也可写入`80`端口，底层传输安全留空

<!-- ![](https://ipfs.io/ipfs/QmRoBPBGmWPRMHYhq2YAAhtfUJKRLYLPo3iy8GsvtbyNrv?2.png) -->

![](https://raw.githubusercontent.com/hoodiearon/fq-book/master/docs/images/2018-05-16_090615.png)

右键设置为活动服务器

<!-- ![](https://ipfs.io/ipfs/QmbDyHz2frv4nEgt4xz1V5TLkg8qc5JjvVnZ2PJSNuYPJF?1.png) -->

![](https://raw.githubusercontent.com/hoodiearon/fq-book/master/docs/images/2018-05-16_091318.png)

测试

<!-- ![](https://ipfs.io/ipfs/QmPkj4HZVJT6QHQVUP4R9yyxk7yhbcSd2zQaRh8PB5Skcr?1.png) -->

![](https://raw.githubusercontent.com/hoodiearon/fq-book/master/docs/images/2018-05-16_093822.png)



