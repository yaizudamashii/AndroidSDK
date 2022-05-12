# Notes

download the arm64 emulator binaries from https://ci.android.com/builds/submitted/7176368/aarch64_sdk_tools_linux/latest/sdk-repo-linux_aarch64-emulator-7176368.zip

download an arm64 system images, website with list of images is https://androidsdkmanager.azurewebsites.net/AndroidSystemImages, image here is https://dl.google.com/android/repository/sys-img/android/arm64-v8a-31_r03.zip

follow the steps in the readme to setup a sdk directory and install "platform-tools" and "platforms;android-31" from the sdkmanager

extract the contents of the arm64 emulator binaries zip to sdk/emulator

extract the contents of the system image downloaded to sdk/system-images/android-31/default/arm64-v8a/

run the emulator with `emulator @test -no-audio -no-boot-anim -no-window -gpu swiftshader_indirect -qemu -cpu max -machine gic-version=max` for headless more. Remove the -no-window to see the emulator window in vnc
