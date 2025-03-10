> [Guides](/Guides.md)/[SnapEnhance](/guides/SnapEnhance.md)

# How to install SnapEnhance (non-root)

## Before we begin
### Warning
By following this process, you acknowledge that any limitation or suspension of your account(s) is not the fault of this document or SnapEnhance - **you choose what you install**.

### Developer Options
You will need to enable *Developer Options*, depending on your phone this prodecure may be different, though the most common way of doing this is as follows:
1. Open *Settings*
2. Navigate to *About Phone*
3. Navigate to *Software Information*
4. Press *Build Number* 7 times

You may be prompted to enter a pin/password, but after this is done you will now have *Developer Options* in *Settings*.

![Image of Developer Options in Settings](/assets/jpg/Screenshot_20240701_021146_Settings.jpg)

## 1. Install requirements from Store
The only requirement from Google Play is [Shizuku](https://play.google.com/store/apps/details?id=moe.shizuku.privileged.api).

## 2. Install requirements from package
You will need three apps from standard packages (.apk)
1. Snapchat v12.81.0.44\* ([nodpi](https://lifix.is-scamming.me/content/cdn/sRLZWLSzBwTP/com.snapchat.android_12.81.0.44-126022_minAPI21(arm64-v8a,armeabi-v7a)(nodpi)_apkmirror.com.apk)) ([160-640dpi](https://lifix.is-scamming.me/content/cdn/ANSCDlAEtAqv/com.snapchat.android_12.81.0.44-126022_2arch_3dpi_14lang_60d3470e93546a3d8996a012a289770d_apkmirror.com.apkm))
2. [LSPatch](https://github.com/xifil/xifil/raw/master/assets/apk/LSPatch-v0.7-430.apk)
3. [SnapEnhance](https://xifil.github.io/se-redirect)

> \* *Snapchat has locked many user accounts that used SnapEnhance or its related forks due to new detections. It's recommended to use Snapchat v12.81.0.44 or earlier. Only use signed builds or builds you've modified yourself to avoid compromising the security of your account.*

For SnapEnhance, ensure you download the latest package correspondant to your devices architecture - the most common one being **ArmV8**. If you are unsure, a simple Google search or Geekbench could help you.

## 3. Configure Shizuku
1. Navigate to *Settings* `>` *Developer Options*, and ensure *Wireless Debugging* is enabled
   ![Wireless Debugging](/assets/jpg/Screenshot_20240701_024052_Settings.jpg)
2. Start the Shizuku pairing process by opening the app, and pressing the *Pairing* button
   ![Pairing](/assets/jpg/Screenshot_20240701_022916_Shizuku.jpg)
3. Go back to *Developer Options* and open *Wireless Debugging* - press *Pair device with pairing code*
   ![Pairing Code Button](/assets/jpg/Screenshot_20240701_023128_Settings.jpg)
4. Shizuku will appear at the top of your screen, **expand** this notification, press *Enter pairing code*, and type out the number at the bottom of your screen. After you confirm it and then press *Start* in Shizuku, Shizuku should be ready to use, you can confirm this by looking at the top of the Shizuku app.
   ![Shizuku Ready](/assets/jpg/Screenshot_20240701_023741_Shizuku.jpg)

## 4. Patch Snapchat
1. Add LSPatch as an authorised app in Shizuku. You can do this by pressing *Tap to manage authorized apps*, then ticking *LSPatch*.
   ![Manage authorized](/assets/jpg/Screenshot_20240701_024615_Shizuku.jpg)
   ![Tick](/assets/jpg/Screenshot_20240701_024626_Shizuku.jpg)
2. Open LSPatch
3. Navigate to the *Manage* tab at the bottom
4. Press the `+` icon in the bottom right, press *OK* when asked for a storage directory
5. Create a new folder and press *Use this folder* at the bottom (mine is `SnapEnhanceLS`)
   ![Folder](/assets/jpg/Screenshot_20240701_031909_My%20Files.jpg)
6. You will be prompted for a new patch, press *Select apk(s) from storage*
7. Find and select the Snapchat `.apk` file you downloaded
8. For the patch mode, select *Integrated* then press *Embed modules*
   ![Embed modules](/assets/jpg/Screenshot_20240701_030128_LSPatch.jpg)
9. Press *Select installed module*, then find and select SnapEnhance
10. Ensure *Override version code* is ticked
    ![Override version code](/assets/jpg/Screenshot_20250107_181336_LSPatch.jpg)
11. Press *Start patch*
12. After it has patched, an *Install* button will appear, press it - it will reinstall Snapchat in a patched state.
13. Back in LSPatch, long press on Snapchat and press *Optimize*
14. Open Snapchat, if the patch was successful you will be prompted to create or find a folder for SnapEnhance to store its media.

## 5. Logging in
When logging in, you most likely will see an error message stating:
> Due to repeated failed attempts or other unusual activity, your access to Snapchat has been temporarily disabled. Learn more here.

To fix this, simply restart the app 3-4 times (only log in when you have restarted it a few times)

## Additional notes
You should now, in the Snapchat app, be able to open the SnapEnhance settings overlay by tapping where it says "Chat" at the very top of the main messages view. Due to it being an overlay, the first open will lead you to the permissions page for on screen overlays, where you'll have to enable SnapEnhance for it to work.
