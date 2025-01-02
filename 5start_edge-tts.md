https://github.com/rany2/edge-tts

```
文本转语音工具

免费使用，无需注册，无限制。
推荐指数5颗星
```

```
pip install edge-tts
edge-tts --text "Hello, world!" --write-media hello.mp3 --write-subtitles hello.srt


```

```
import edge_tts

TEXT = "Hello World!"
VOICE = "en-GB-SoniaNeural"
OUTPUT_FILE = "test.mp3"


def main() -> None:
    """Main function"""
    communicate = edge_tts.Communicate(TEXT, VOICE)
    communicate.save_sync(OUTPUT_FILE)


if __name__ == "__main__":
    main()
```
