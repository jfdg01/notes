# How to create an APK

### 1. **Generate Your Project Using gdx-liftoff**

### 2. **Open the Project in Android Studio**

### 3. **Build the APK Using Gradle**

1. Open a terminal or Command Prompt.
2. Navigate to the root directory (where `android`, `lwjgl3` and `core` is) 
3. Run the Gradle build command:
    
    ```bash
    ./gradlew assembleDebug
    ```
    
4. Once the build is complete, you will find the APK in the `android/build/outputs/apk/debug/` directory.

### 4. **Prepare Your Android Device FOR DEBUGGING**

1. Connect via USB or download via web (if option exists)
2. Move the APK to the Downloads forlder and give proper permissions to install