安装php－version
-------------

此时我们再安装php－version ==\> php版本切换工具
安装命令：

    1
    2

    brew install php-version
    source $(brew --prefix php-version)/php-version.sh && php-version 5

执行php－version查看已存在的php版本,前面带＊的是当前环境正在使用的php版本,使用php－versiom＋版本号的方式切换php版本～

    1
    2
    3
    4
    5
    6
    7
    8
    9
    10

    localhost:~ Ken$ php-version
     5.5.30
    \* 5.6.17
     7.0.2
    localhost:~ Ken$ php-version 7.0.2
    localhost:~ Ken$ php -v
    PHP 7.0.2 (cli) (built: Jan 7 2016 10:40:26) ( NTS )
    Copyright (c) 1997-2015 The PHP Group
    Zend Engine v3.0.0, Copyright (c) 1998-2015 Zend Technologies
    localhost:~ Ken$