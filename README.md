# 自言自语
IG啊IG，今年你还有机会吗
效果图：
第一排TheShy，Duke，Ning，Rookie，JackeyLove
第三排中间三个Baolan~
是我最喜欢的18極了
**source images:**
![](https://ai-studio-static-online.cdn.bcebos.com/a9c6f640a5ae4f89a4ffa19bb55754d213e659e6ec5c4fca94d284373e33868f)
**generated images:**
![](https://ai-studio-static-online.cdn.bcebos.com/719712e91eae44269498c55ef3786a93de1882155c284b72b6a9f57c056262c1)

# 安装paddlehub环境
安装paddlehub


```python
# 如果需要进行持久化安装, 需要使用持久化路径, 如下方代码示例:
# If a persistence installation is required, 
# you need to use the persistence path as the following: 
!pip install paddlehub==2.0.0b2
```

    Looking in indexes: https://mirror.baidu.com/pypi/simple/
    Collecting paddlehub==2.0.0b2
    [?25l  Downloading https://mirror.baidu.com/pypi/packages/ca/1c/a0304ed4ce0ee694f4d9d2ee35dc335a0359ad43eb9ddb8f687fb032a91c/paddlehub-2.0.0b2-py3-none-any.whl (197kB)
    [K     |████████████████████████████████| 204kB 13.0MB/s eta 0:00:01
    [?25hRequirement already satisfied: colorlog in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from paddlehub==2.0.0b2) (4.1.0)
    Requirement already satisfied: numpy in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from paddlehub==2.0.0b2) (1.16.4)
    Requirement already satisfied: tqdm in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from paddlehub==2.0.0b2) (4.36.1)
    Requirement already satisfied: colorama in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from paddlehub==2.0.0b2) (0.4.4)
    Requirement already satisfied: packaging in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from paddlehub==2.0.0b2) (20.9)
    Requirement already satisfied: pyyaml in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from paddlehub==2.0.0b2) (5.1.2)
    Requirement already satisfied: visualdl>=2.0.0 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from paddlehub==2.0.0b2) (2.1.1)
    Requirement already satisfied: opencv-python in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from paddlehub==2.0.0b2) (4.1.1.26)
    Requirement already satisfied: gitpython in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from paddlehub==2.0.0b2) (3.1.14)
    Requirement already satisfied: paddlenlp>=2.0.0b in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from paddlehub==2.0.0b2) (2.0.0rc7)
    Requirement already satisfied: gunicorn>=19.10.0; sys_platform != "win32" in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from paddlehub==2.0.0b2) (20.0.4)
    Requirement already satisfied: filelock in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from paddlehub==2.0.0b2) (3.0.12)
    Requirement already satisfied: matplotlib in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from paddlehub==2.0.0b2) (2.2.3)
    Requirement already satisfied: pyzmq in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from paddlehub==2.0.0b2) (18.1.1)
    Requirement already satisfied: easydict in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from paddlehub==2.0.0b2) (1.9)
    Requirement already satisfied: flask>=1.1.0 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from paddlehub==2.0.0b2) (1.1.1)
    Requirement already satisfied: rarfile in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from paddlehub==2.0.0b2) (3.1)
    Requirement already satisfied: Pillow in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from paddlehub==2.0.0b2) (7.1.2)
    Requirement already satisfied: pyparsing>=2.0.2 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from packaging->paddlehub==2.0.0b2) (2.4.2)
    Requirement already satisfied: protobuf>=3.11.0 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from visualdl>=2.0.0->paddlehub==2.0.0b2) (3.14.0)
    Requirement already satisfied: Flask-Babel>=1.0.0 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from visualdl>=2.0.0->paddlehub==2.0.0b2) (1.0.0)
    Requirement already satisfied: bce-python-sdk in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from visualdl>=2.0.0->paddlehub==2.0.0b2) (0.8.53)
    Requirement already satisfied: requests in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from visualdl>=2.0.0->paddlehub==2.0.0b2) (2.22.0)
    Requirement already satisfied: pre-commit in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from visualdl>=2.0.0->paddlehub==2.0.0b2) (1.21.0)
    Requirement already satisfied: shellcheck-py in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from visualdl>=2.0.0->paddlehub==2.0.0b2) (0.7.1.1)
    Requirement already satisfied: flake8>=3.7.9 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from visualdl>=2.0.0->paddlehub==2.0.0b2) (3.8.2)
    Requirement already satisfied: six>=1.14.0 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from visualdl>=2.0.0->paddlehub==2.0.0b2) (1.15.0)
    Requirement already satisfied: gitdb<5,>=4.0.1 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from gitpython->paddlehub==2.0.0b2) (4.0.5)
    Requirement already satisfied: seqeval in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from paddlenlp>=2.0.0b->paddlehub==2.0.0b2) (1.2.2)
    Requirement already satisfied: h5py in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from paddlenlp>=2.0.0b->paddlehub==2.0.0b2) (2.9.0)
    Requirement already satisfied: jieba in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from paddlenlp>=2.0.0b->paddlehub==2.0.0b2) (0.42.1)
    Requirement already satisfied: setuptools>=3.0 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from gunicorn>=19.10.0; sys_platform != "win32"->paddlehub==2.0.0b2) (41.4.0)
    Requirement already satisfied: cycler>=0.10 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from matplotlib->paddlehub==2.0.0b2) (0.10.0)
    Requirement already satisfied: pytz in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from matplotlib->paddlehub==2.0.0b2) (2019.3)
    Requirement already satisfied: kiwisolver>=1.0.1 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from matplotlib->paddlehub==2.0.0b2) (1.1.0)
    Requirement already satisfied: python-dateutil>=2.1 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from matplotlib->paddlehub==2.0.0b2) (2.8.0)
    Requirement already satisfied: Werkzeug>=0.15 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from flask>=1.1.0->paddlehub==2.0.0b2) (0.16.0)
    Requirement already satisfied: Jinja2>=2.10.1 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from flask>=1.1.0->paddlehub==2.0.0b2) (2.10.1)
    Requirement already satisfied: click>=5.1 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from flask>=1.1.0->paddlehub==2.0.0b2) (7.0)
    Requirement already satisfied: itsdangerous>=0.24 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from flask>=1.1.0->paddlehub==2.0.0b2) (1.1.0)
    Requirement already satisfied: Babel>=2.3 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from Flask-Babel>=1.0.0->visualdl>=2.0.0->paddlehub==2.0.0b2) (2.8.0)
    Requirement already satisfied: pycryptodome>=3.8.0 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from bce-python-sdk->visualdl>=2.0.0->paddlehub==2.0.0b2) (3.9.9)
    Requirement already satisfied: future>=0.6.0 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from bce-python-sdk->visualdl>=2.0.0->paddlehub==2.0.0b2) (0.18.0)
    Requirement already satisfied: certifi>=2017.4.17 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from requests->visualdl>=2.0.0->paddlehub==2.0.0b2) (2019.9.11)
    Requirement already satisfied: urllib3!=1.25.0,!=1.25.1,<1.26,>=1.21.1 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from requests->visualdl>=2.0.0->paddlehub==2.0.0b2) (1.25.6)
    Requirement already satisfied: idna<2.9,>=2.5 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from requests->visualdl>=2.0.0->paddlehub==2.0.0b2) (2.8)
    Requirement already satisfied: chardet<3.1.0,>=3.0.2 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from requests->visualdl>=2.0.0->paddlehub==2.0.0b2) (3.0.4)
    Requirement already satisfied: virtualenv>=15.2 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from pre-commit->visualdl>=2.0.0->paddlehub==2.0.0b2) (16.7.9)
    Requirement already satisfied: cfgv>=2.0.0 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from pre-commit->visualdl>=2.0.0->paddlehub==2.0.0b2) (2.0.1)
    Requirement already satisfied: importlib-metadata; python_version < "3.8" in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from pre-commit->visualdl>=2.0.0->paddlehub==2.0.0b2) (0.23)
    Requirement already satisfied: nodeenv>=0.11.1 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from pre-commit->visualdl>=2.0.0->paddlehub==2.0.0b2) (1.3.4)
    Requirement already satisfied: toml in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from pre-commit->visualdl>=2.0.0->paddlehub==2.0.0b2) (0.10.0)
    Requirement already satisfied: identify>=1.0.0 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from pre-commit->visualdl>=2.0.0->paddlehub==2.0.0b2) (1.4.10)
    Requirement already satisfied: aspy.yaml in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from pre-commit->visualdl>=2.0.0->paddlehub==2.0.0b2) (1.3.0)
    Requirement already satisfied: mccabe<0.7.0,>=0.6.0 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from flake8>=3.7.9->visualdl>=2.0.0->paddlehub==2.0.0b2) (0.6.1)
    Requirement already satisfied: pycodestyle<2.7.0,>=2.6.0a1 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from flake8>=3.7.9->visualdl>=2.0.0->paddlehub==2.0.0b2) (2.6.0)
    Requirement already satisfied: pyflakes<2.3.0,>=2.2.0 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from flake8>=3.7.9->visualdl>=2.0.0->paddlehub==2.0.0b2) (2.2.0)
    Requirement already satisfied: smmap<4,>=3.0.1 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from gitdb<5,>=4.0.1->gitpython->paddlehub==2.0.0b2) (3.0.5)
    Requirement already satisfied: scikit-learn>=0.21.3 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from seqeval->paddlenlp>=2.0.0b->paddlehub==2.0.0b2) (0.22.1)
    Requirement already satisfied: MarkupSafe>=0.23 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from Jinja2>=2.10.1->flask>=1.1.0->paddlehub==2.0.0b2) (1.1.1)
    Requirement already satisfied: zipp>=0.5 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from importlib-metadata; python_version < "3.8"->pre-commit->visualdl>=2.0.0->paddlehub==2.0.0b2) (0.6.0)
    Requirement already satisfied: joblib>=0.11 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from scikit-learn>=0.21.3->seqeval->paddlenlp>=2.0.0b->paddlehub==2.0.0b2) (0.14.1)
    Requirement already satisfied: scipy>=0.17.0 in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from scikit-learn>=0.21.3->seqeval->paddlenlp>=2.0.0b->paddlehub==2.0.0b2) (1.3.0)
    Requirement already satisfied: more-itertools in /opt/conda/envs/python35-paddle120-env/lib/python3.7/site-packages (from zipp>=0.5->importlib-metadata; python_version < "3.8"->pre-commit->visualdl>=2.0.0->paddlehub==2.0.0b2) (7.2.0)
    Installing collected packages: paddlehub
      Found existing installation: paddlehub 2.0.4
        Uninstalling paddlehub-2.0.4:
          Successfully uninstalled paddlehub-2.0.4
    Successfully installed paddlehub-2.0.0b2


# 数据准备
准备了几张照片（19春季赛的定妆照
![](https://ai-studio-static-online.cdn.bcebos.com/ed6bf73a8cdd431fac8793f5c3ca08004f261c550ef34871901423bfb38b374c)
![](https://ai-studio-static-online.cdn.bcebos.com/760a10c796f949a6a0b03130ab0de17cc01a74c7313344c48706c791bb93b77c)
![](https://ai-studio-static-online.cdn.bcebos.com/afe01dbf777e42dcba7a95d5805c5069752fa03b5fb8462d824b617df6ff4318)
![](https://ai-studio-static-online.cdn.bcebos.com/eaf61b2270b84b31aaf7a099050d19827bda1001d6dc431d8f422c995a23d3cb)
![](https://ai-studio-static-online.cdn.bcebos.com/26d1b9295d664050a2a7308699c82949560797042e3a432b8c9f6d113bc1564b)
![](https://ai-studio-static-online.cdn.bcebos.com/ceab6b7cd2b84fa98cd308450f223a7df7d6d61d6ca34044ac832fdb24a09e92)

# 导入U2Net_Portrait模型
项目采用了U2Net_Portrait网络。从PaddleHub里导入了预训练模型


```python
import paddlehub as hub
import os
import cv2

os.environ["CUDA_VISIBLE_DEVICES"] = "0"
# 模型加载
# use_gpu：是否使用GPU进行预测
for f in os.listdir('./18ji'):
    model = hub.Module(name='U2Net_Portrait')
    # img = cv2.imread(os.path.join('./18ji', f))
    # result = model.Cartoon_GEN(images=[img], output_dir='./output_frames')
    result = model.Portrait_GEN(images=[img], output_dir='./output_frames2')
    # print(result[0].shape)
    cv2.imwrite(f'./18ji_output/{f}', result[0])
```

    146.0


![](https://ai-studio-static-online.cdn.bcebos.com/2625bf36fb154b588f17b88c40c3dff29a8c67992c784670afdd87ebf504ff56)
![](https://ai-studio-static-online.cdn.bcebos.com/ed638b05becc47e4b2740cdb148156fbe1aae83b11ff4100bdda333e0f9c15bf)
![](https://ai-studio-static-online.cdn.bcebos.com/556c195e315549dbbd519a00a88b3fa012cf9de569f04d87984e432d5d5ba6d4)
![](https://ai-studio-static-online.cdn.bcebos.com/22ea6474e5c14c8dbed57467e51b49c06f78b54e951d494aa2614d56d0aa433d)
![](https://ai-studio-static-online.cdn.bcebos.com/8a2e7fee27c9477f942f1cf6486511bd554634e48a054253b5837c226f9c9d34)
![](https://ai-studio-static-online.cdn.bcebos.com/92979f19e44e4fddb498b9cd8767b58150fca99a97544f5bae22f714eb82438d)
![](https://ai-studio-static-online.cdn.bcebos.com/aade7d1b9f19485e87c70c583f7199ea836eabcd81b54255a1d3ebb3986ea4ff)

\（呜呜呜shy哥好帅我要放两张）


# 合成为一张图


```python
import cv2
import numpy as np
import os

root = './18ji_output'
w, h = 128, 128
cnt_h = 4
cnt_w = 5
res = np.zeros((h * cnt_h, w * cnt_w, 3))
now_h = 0
now_w = 0
for path in os.listdir(root):
    path = os.path.join(root, path)
    img = cv2.resize(cv2.imread(path), (w, h))
    # cv2.imwrite('f.png', img)
    # print(now_h * h, (now_h + 1) * h)
    res[now_h * h: (now_h + 1) * h, now_w * w: (now_w + 1) * w, :] = img
    now_w += 1
    if now_w == cnt_w:
        now_w = 0
        now_h += 1

cv2.imwrite('res.png', res)
```




    True



![](https://ai-studio-static-online.cdn.bcebos.com/719712e91eae44269498c55ef3786a93de1882155c284b72b6a9f57c056262c1)

