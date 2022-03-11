# MaskRCNN_TF2

MaskRCNN 在TF2.x情况下跑通自己的数据集
* mrcnn 替换掉官方的mrcnn文件夹即可开箱使用
* labelme2coco 将labelme打标工具生成的json变成coco形式的json文件


* 训练：`python train.py train --dataset=./dataset --weights=coco` （注意这里要把数据集放在dataset目录下哦）
* 预测：`python pred.py`

在win10+gpu rtx3090跑通。替换maskrcnn_tf1的mrcnn里的全部文件，注意调小Batch size，即调小IMAGES_PER_GPU,本项目测试是8，太大会提示内存耗尽。
(py36_maskrcnn_env_bak) C:\Users\dell>pip list
Package                  Version
------------------------ -------------------
absl-py                  0.15.0
astor                    0.8.1
astunparse               1.6.3
backcall                 0.2.0
bleach                   1.5.0
cached-property          1.5.2
cachetools               4.2.4
certifi                  2020.6.20
charset-normalizer       2.0.9
clang                    5.0
colorama                 0.4.4
cycler                   0.11.0
Cython                   0.29.28
dataclasses              0.8
decorator                4.4.2
flatbuffers              1.12
gast                     0.4.0
google-auth              1.35.0
google-auth-oauthlib     0.4.6
google-pasta             0.2.0
grpcio                   1.44.0
h5py                     3.1.0
html5lib                 0.9999999
idna                     3.3
imageio                  2.13.5
imgaug                   0.4.0
imgviz                   1.4.1
importlib-metadata       4.8.3
ipython                  7.16.2
ipython-genutils         0.2.0
jedi                     0.17.2
keras                    2.6.0
Keras-Applications       1.0.8
Keras-Preprocessing      1.1.2
kiwisolver               1.3.1
labelme                  3.16.2
libclang                 11.1.0
Markdown                 3.3.6
matplotlib               3.2.2
mock                     4.0.3
networkx                 2.5.1
numpy                    1.19.5
nvidia-pyindex           1.0.9
oauthlib                 3.1.1
opencv-python            4.5.4.60
opt-einsum               3.3.0
packaging                21.3
parso                    0.7.1
pickleshare              0.7.5
Pillow                   8.3.2
pip                      21.2.2
prompt-toolkit           3.0.24
protobuf                 3.17.3
pyasn1                   0.4.8
pyasn1-modules           0.2.8
Pygments                 2.10.0
pyparsing                3.0.6
PyQt5                    5.15.6
PyQt5-Qt5                5.15.2
PyQt5-sip                12.9.0
python-dateutil          2.8.2
PyWavelets               1.1.1
PyYAML                   6.0
QtPy                     1.9.0
requests                 2.26.0
requests-oauthlib        1.3.0
rsa                      4.8
scikit-image             0.16.2
scipy                    1.4.1
setuptools               58.0.4
Shapely                  1.8.1.post1
six                      1.15.0
tb-nightly               2.6.0a20210806
tensorboard              2.6.0
tensorboard-data-server  0.6.1
tensorboard-plugin-wit   1.8.1
tensorflow               2.6.0
tensorflow-estimator     2.6.0
tensorflow-gpu           2.6.2
tensorflow-gpu-estimator 2.2.0
termcolor                1.1.0
tf-estimator-nightly     2.7.0.dev2021092408
tifffile                 2020.9.3
traitlets                4.3.3
typing-extensions        3.7.4.3
urllib3                  1.26.7
wcwidth                  0.2.5
Werkzeug                 2.0.2
wheel                    0.37.0
wincertstore             0.2
wrapt                    1.12.1
zipp                     3.6.0





>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
maskrcnn_tf1.x 资料如下：
win10 + python 3.6.9 Tensorflow 1.15.0 keras  2.2.5 Pillow 5.3.0 + cpu已经跑通代码：https://github.com/junlintianxiatjm/Mask_RCNN-master007







