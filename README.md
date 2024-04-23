# 2024

```shell
# Compress Audio
ffmpeg -i input_audio.wav -c:a aac -b:a 128k output_audio.aac
```

```shell
# Convert to HLS
ffmpeg -i input_audio.aac -c:a copy -f hls -hls_time 10 -hls_list_size 0 output.m3u8
```
