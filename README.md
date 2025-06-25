# MY-LLM Project

This repository contains an Android application demonstrating on-device language model integration.

## Modules
- **M1Model**: Example TensorFlow Lite model wrapper located in `app/src/main/java/com/example/myllmapp/M1Model.kt`.
- **MainActivity**: UI with Google login and buttons to invoke M1 (text) and placeholder M2 models.

The project uses Gradle to build and run unit tests:

```bash
./gradlew test
```

Note: The project relies on TensorFlow Lite. Gradle will fetch the
`org.tensorflow:tensorflow-lite` dependency when you build the app.
If network access is restricted, configure a local Maven cache or
download the library manually before running Gradle.
