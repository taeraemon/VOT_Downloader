Currently on working

## VOT Downloader
```
VOT Challenge에 쓰이는 데이터셋을 나름 쉽게 다운로드하기 위한 레포입니다.
```

### 1. Environment Setup
```
12900KF, 2*A6000, ubuntu22.04
pyenv+venv 기준

git clone https://github.com/taeraemon/VOT_Downloader.git
cd VOT_Downloader

pyenv install 3.7.6
pyenv global 3.7.6
python3 -m venv env
source env/bin/activate

pip install tqdm six requests
```
```
Package            Version
------------------ ---------
certifi            2024.8.30
charset-normalizer 3.4.0
idna               3.10
pip                19.2.3
requests           2.31.0
setuptools         41.2.0
six                1.17.0
tqdm               4.67.1
urllib3            2.0.7
```
&nbsp;


### 2. Run script
```
assuming you are in /VOT_DOWNLOADER
python3 run.py
```
&nbsp;


### 3. Result
```
(env) tykim@tySM:~/Documents/Python/down_VOT2018$ python3 test.py
                      |                                                              |   0% [00:00<?]ants1.zip
 Downloading          |█▏                                                           |   2% [00:17<17:03]ants3.zip
 Downloading          |██▍                                                          |   3% [01:12<38:21]bag.zip
 Downloading          |███▋                                                         |   5% [01:20<23:40]ball1.zip
 .
 .
 .
 Downloading          |███████████████████████████████████████████████████████████████████████▊ |  98% [15:31<00:09]zebrafish1.zip
 Downloading          |█████████████████████████████████████████████████████████████████████████| 100% [15:46<00:00]
```
```
VOT_Downloader
    ...
    /dataset
        /VOT
            /ants1
                /color
                    00000001.jpg
                    ...
                camera_motion.tag
                ...
                size_change.tag
            /ants3
                ...
            ...
            /zebrafish1
            list.txt
    ...
```
