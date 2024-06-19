1. To create an apk run the command `gradlew android:assembleRelease` -- This will create a file named `android-release-unsigned.apk` at the directory `build/outputs/apk/release/`.
2. Now run the `apksigner` command with correct credentials.
  > To create a key run the command: `keytool -genkey -v -keystore "signing-key.jks" -keyalg RSA -keysize 2048 -validity 10000 -alias "kandclay"`. If this doesn't work try not using the quotes. **IMPORTANT**: Remember the alias.
3. Run the command with the correct directories: `apksigner sign --ks "C:\Users\gara\Documents\keys\signing-key.jks" --ks-key-alias "kandclay" --out "C:\Users\gara\Documents\LibGDX Proyects\CBClone\android\build\outputs\apk\release\TestGame.apk" "C:\Users\gara\Documents\LibGDX Proyects\CBClone\android\build\outputs\apk\release\android-release-unsigned.apk"`.
4. It will generate a signed apk in the same directory named "TestGame.apk" in this case. 
