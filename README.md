#### TEST REPO LINKS ###
rm -rf packages/apps/Settings && git clone https://github.com/afterallafk/packages_apps_Settings-1.git -b 12.1 packages/apps/Settings && rm -rf frameworks/base && git clone https://github.com/afterallafk/frameworks_base-1.git -b 12.1 frameworks/base && rm -rf packages/apps/BlazeHouse && git clone https://github.com/afterallafk/packages_apps_BlazeHouse.git -b 12.1 packages/apps/BlazeHouse 

### HALS ###
rm -rf hardware/qcom-caf/msm8996/audio && rm -rf hardware/qcom-caf/msm8996/media && rm -rf hardware/qcom-caf/msm8996/display && rm -rf hardware/qcom-caf/wlan && git clone https://github.com/afterallafk/hardware_qcom-caf_msm8996_audio.git -b 12 hardware/qcom-caf/msm8996/audio && git clone https://github.com/afterallafk/hardware_qcom-caf_msm8996_media.git -b 12 hardware/qcom-caf/msm8996/media && git clone https://github.com/afterallafk/hardware_qcom-caf_msm8996_display.git -b 12 hardware/qcom-caf/msm8996/display && git clone https://github.com/afterallafk/hardware_qcom-caf_wlan.git -b 12 hardware/qcom-caf/wlan

### DEVICE SOURCES ###
git clone https://github.com/ProjectBlaze-Devices/device_xiaomi_onclite -b 12.1 device/xiaomi/onclite && git clone https://github.com/afterallafk/vendor_xiaomi_onclite-12.git -b twelve vendor/xiaomi/onclite && git clone https://github.com/afterallafk/kernel_xiaomi_onclite.git -b 12.1 kernel/xiaomi/onclite && . build/envsetup.sh && lunch blaze_onclite-userdebug && make bacon
