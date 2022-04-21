# rtaudio熟悉


#### 自带小工具
+ apinames  
  名称和API之间的转换(使用的Audio库)。
+ audioprobe
  打印音频设备信息。
+ duplex
+ playraw
+ playsaw
+ record 录音，然后使用playraw播放。
    ```shell
    # 1 是录音的通道数量，44100是采样率
    ./record 1 44100
    ```  