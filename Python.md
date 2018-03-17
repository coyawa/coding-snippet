































Pip update all packages

```
pip install -U $(pip freeze | awk '{split($0, a, "=="); print a[1]}')
```

```

```



Tips-Python

[nschloe/pipdated: Python module for checking for updates on PyPi.](https://github.com/nschloe/pipdated)

[虚拟环境 — Python最佳实践指南](http://pythonguidecn.readthedocs.io/zh/latest/dev/virtualenvs.html) virtualenv

Curl http… \> reddit.json

More reddit.json

![Pasted Graphic 1.tiff](resources/E1B2E9B7B2321B9DDCA2C631F67EAF7C.jpg)

Like pretty()

![Pasted Graphic.tiff](resources/1A1B6D86D457D21F537495A0A1CF83A4.jpg)

```python
for python 3
pip install bottle
For python 2
Sudo python -m easy_install bottle


Sudo python2.7 -m pip install scipy
//if the eviroment already has the python 2 and python 3, use this command to install the package

py -2.7

Upgrade python2 package
sudo python2.7 -m pip install --upgrade numpy

pip2 freeze --local | grep -v '^\-e' | cut -d = -f 1  | xargs pip2 install -U


# Use Homebrew :)
brew install python3
# To update it:
brew update
brew upgrade python3
```



\#\#读取json文件并转换为字典

```python
# -*- coding:utf-8 -*-
import json
file_path = 'json文件相对路径或者据对路径'
with open(file_path) as f:
    js = json.load(f)  # js是转换后的字典
```



















