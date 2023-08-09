# Yating ASR Transcription SDK - Java version

## Available Key

- Please contact Yating ASR

### Input

```JSON
{
    "audioUri": "http://www.example.com/audio.mp3",
    "modelConfig": {
        "model": "asr-zh-en-std",
        "customLm": ""
    },
    "featureConfig": {
        "punctuation": true,
        "speakerDiarization": true,
        "speakerCount": 0,
        "sentiment": true
    }
}
```

## Available Variable

### Audio Uri

可使用的音檔網址。

### Model Config

| Name     | Data Type | Description                       |
| -------- | --------- | --------------------------------- |
| model    | String    | 語言模型，請參考下方 model 設定。 |
| customLm | String    | 客製化模型，若無則預設空白。      |

### Model

| Name          | Description                        |
| ------------- | ---------------------------------- |
| asr-zh-en-std | 中文為主，並可處理英文夾雜的情況。 |
| asr-zh-tw-std | 中文為主，並可處理台語夾雜的情況。 |
| asr-en-std    | 全英文情境使用。                   |

### Feature Config

| Name               | Data Type | Description                                                                              |
| ------------------ | --------- | ---------------------------------------------------------------------------------------- |
| punctuation        | Boolean   | 標點符號，預設為 true。                                                                  |
| speakerDiarization | Boolean   | 語者辨識，預設為 true。                                                                  |
| speakerCount       | Integer   | 語者數量，開啟語者辨識後，提供語者數量可讓語者辨識結果更為準確，未提供則讓模型自行辨識。 |
| sentiment          | Boolean   | 情緒辨識，預設為 true。                                                                  |
