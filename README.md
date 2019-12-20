## [原始的代码](https://github.com/rbgirshick/py-faster-rcnn) 
从上面的网址下载的，改正了几个小错误，主要是python的包的版本不兼容导致的

### 1.下载代码

```Shell
git clone https://github.com/zhaowujie/py-faster-rcnn.git
```

### 2.解压根目录下的文件夹
```Shell
cd 到lib 		make
cd 到caffe-fast-rcnn	make -j8 && make pycaffe
```

### 3.训练
```Shell
python2 tools/train_net.py --solver /path/to/sovler.prototxt --weights /path/to/pre-trained/model --cfg /path/to/cfg.yml 
```
### 4.测试
```Shell
python2 tools/test_net.py --def /path/to/test.prototxt --net /path/to/caffemodel --cfg /path/to/cfg.yml 
```
### 5.演示
```Shell
cd $FRCN_ROOT
python2 ./tools/demo.py
```
