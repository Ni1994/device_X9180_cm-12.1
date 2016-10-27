local_manifests/roomservice.xml for CM12.1:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>

  <project name="CyanogenMod/android_device_qcom_common" path="device/qcom/common" remote="github" revision="cm-12.1" />
  <project name="CyanogenMod/android_hardware_qcom_fm" path="hardware/qcom/fm" remote="github" revision="cm-12.1" />

  <project name="Ni1994/device_X9180_cm-12.1.git" path="frameworks/av/media/libstagefright/data" remote="github" revision="media" />
  <project name="Ni1994/kernel_X9180_cm-12.1" path="kernel/ZTE/X9180" remote="github" revision="cm12.1" />
  <project name="Ni1994/device_X9180_cm-12.1" path="device/ZTE/X9180" remote="github" revision="cm12.1" />
  <project name="Ni1994/vendor_X9180_cm-12.1.git" path="vendor/ZTE/X9180" remote="github" revision="cm12.1" />
</manifest>
```
build command
```xml
source build/envsetup.sh
lunch cm_X9180-userdebug
brunch X9180
```
