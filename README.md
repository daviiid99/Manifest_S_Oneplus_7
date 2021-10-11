# ONEPLUS 7 | Build Instructions with Manifest
<br/>

Initialize LineageOS repo:
```
mkdir -p ~/android/lineage
cd ~/android/lineage
repo init https://github.com/daviiid99/Manifest_S_Oneplus_7.git -b Manifest_S
```
<br/>

Sync repo:
```
repo sync
source build/envsetup.sh
```
<br/>

Build:
```
lunch lineage_guacamoleb-userdebug
make bacon
```

<br/>
