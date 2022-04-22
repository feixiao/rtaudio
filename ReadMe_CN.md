# rtaudio熟悉


#### 自带小工具
+ apinames  
  名称和API之间的转换(使用的Audio库)。
+ audioprobe
  打印音频设备信息。
+ duplex
+ playraw 播放record采集的PCM数据
```shell
# 播放record采集的PCM
./tests/playraw  1 48000 ./record.raw 
```
+ playsaw
+ record 录音保存PCM数据，然后使用playraw播放。
    ```shell
    # 1 是录音的通道数量
    # 48000 是采样率
    # 5.0 是时间
    # 1 是 设备
    ./tests/record 1 48000 5.0 1

    # 直接播放PCM
    ffplay -ar 48000 -channels 1 -f s16le  record.raw 
    ```  