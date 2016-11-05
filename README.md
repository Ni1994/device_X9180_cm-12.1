local_manifests/roomservice.xml for CM12.1:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>

  <project name="CyanogenMod/android_device_qcom_common" path="device/qcom/common" remote="github" revision="cm-12.1" />
  <project name="CyanogenMod/android_hardware_qcom_fm" path="hardware/qcom/fm" remote="github" revision="cm-12.1" />

  <project name="Ni1994/kernel_X9180_cm-12.1.git" path="kernel/ZTE/X9180" remote="github" />
  <project name="Ni1994/device_X9180_cm-12.1.git" path="device/ZTE/X9180" remote="github"  />
  <project name="Ni1994/vendor_X9180_cm-12.1.git" path="vendor/ZTE/X9180" remote="github" />
</manifest>
```
将"device_X9180_cm-12.1/mdeia/media_codecs_ffmpeg.xml"复制到"frameworks/av/media/libstagefright/data"<br>
build command
```xml
source build/envsetup.sh
lunch cm_X9180-userdebug
brunch X9180
```
ubuntu16.04编译时注释掉"kernel/ZTE/X9180/kernel/timeconst.pl"里的
```xml
	if (!defined(@val)) {
		@val = compute_values($hz);
	}
```

