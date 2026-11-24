# SocialKosher model files

Model files the SocialKosher app downloads when needed. Nothing else lives here.

| File | What it is | Licence |
|---|---|---|
| `siglip_vision_b32_int8.tflite` (release `siglip-cpu-2026-11-15`) | The image encoder of Google's SigLIP 2 B/32 (256 px), converted to 8-bit TensorFlow Lite to run on an iPhone's processor. The app downloads it only on an iPhone whose built-in fast copy doesn't pass its accuracy check. | Apache License 2.0 (Google's [SigLIP 2 model card](https://huggingface.co/google/siglip2-base-patch32-256)); see `LICENSE` |

The app checks the file's size and SHA-256 before using it:

- size: 95,851,040 bytes
- SHA-256: `e093714aefa075c80ee9fed327dffadd9ac1c35ff935a75857d2c169579d116a`

SigLIP 2 was made by Google. This repository only converts and hosts the vision part; it is not affiliated with
or endorsed by Google.
