# GlobalWebinspect

Enable WebView inspector for all iOS apps, requires jailbreak

## Usage

* Enable WebInspector in Preferences
* Build and install the tweak `THEOS_DEVICE_IP=localhost THEOS_DEVICE_PORT=2222 make package install`
* Re-plug the USB cable and restart target app

## package and install log

```text
macbook@admin GlobalWebInspect % make package install
> Making all for tweak webinspect…
==> Preprocessing Tweak.xm…
==> Compiling Tweak.xm (armv7)…
==> Linking tweak webinspect (armv7)…
==> Generating debug symbols for webinspect…
rm ~/Workspace/OpenSource/GlobalWebInspect/.theos/obj/debug/armv7/Tweak.xm.mm
==> Preprocessing Tweak.xm…
==> Compiling Tweak.xm (arm64)…
==> Linking tweak webinspect (arm64)…
==> Generating debug symbols for webinspect…
rm ~/Workspace/OpenSource/GlobalWebInspect/.theos/obj/debug/arm64/Tweak.xm.mm
==> Preprocessing Tweak.xm…
==> Compiling Tweak.xm (arm64e)…
==> Linking tweak webinspect (arm64e)…
==> Generating debug symbols for webinspect…
rm ~/Workspace/OpenSource/GlobalWebInspect/.theos/obj/debug/arm64e/Tweak.xm.mm
==> Merging tweak webinspect…
==> Signing webinspect…
> Making stage for tweak webinspect…
dm.pl: building package `me.chichou.webinspect-global:iphoneos-arm' in `./packages/me.chichou.webinspect-global_0.1.0-1+debug_iphoneos-arm.deb'
==> Installing…
root@127.0.0.1's password:
dpkg: warning: downgrading me.chichou.webinspect-global from 0.1.0-2+debug to 0.1.0-1+debug
(Reading database ... 1866 files and directories currently installed.)
Preparing to unpack /tmp/_theos_install.deb ...
Unpacking me.chichou.webinspect-global (0.1.0-1+debug) over (0.1.0-2+debug) ...
Setting up me.chichou.webinspect-global (0.1.0-1+debug) ...
install.exec "launchctl stop com.apple.webinspectord"
root@127.0.0.1's password:
echo you need to kill the target App and restart Safari to make it work
you need to kill the target App and restart Safari to make it work
```
