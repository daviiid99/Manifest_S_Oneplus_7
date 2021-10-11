# ONEPLUS 7 | Build Instructions with Manifest
<br/>

Initialize LineageOS repo:
```
mkdir -p ~/android/lineage
cd ~/android/lineage
repo init https://github.com/daviiid99/Manifest_S_Oneplus_7.git -b Manifest_S
```
<br/>

Download repos:
```
mkdir -p .repo/local_manifests
curl https://raw.githubusercontent.com/daviiid99/Manifest_S_Oneplus_7/Manifest_S/snippets/oneplus.xml > .repo/local_manifests/guacamoleb.xml
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
