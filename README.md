# MY-LLM Project

This repository contains an Android application demonstrating on-device language model integration.

## Modules
- **M1Model**: Example TensorFlow Lite model wrapper located in `app/src/main/java/com/example/myllmapp/M1Model.kt`.
- **MainActivity**: UI with Google login and buttons to invoke M1 (text) and placeholder M2 models.

The project uses Gradle to build and run unit tests:

```bash
./gradlew test
```

Note: To allow offline builds, minimal TensorFlow Lite stub classes are
included in the source tree. They provide just enough API for the app to
compile without the real TensorFlow Lite runtime. Replace them with the
actual `org.tensorflow:tensorflow-lite` library when you need real
model inference.
