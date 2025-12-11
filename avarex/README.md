# AvareX 0.68-based Android/Windows versions

[2005-12-11]<br>
This version of AvareX is derived from the main AvareX-0.0.68+68 version (prior to recent AI additions) but with the following modifications:
* **Functional NOTAMS** using published FAA API on https://notams.aim.faa.gov/notamSearch/.  See [PR #93](https://github.com/apps4av/avarex/pull/93)

* **METARs tab when not Kxxx** (e.g. 42J, X60).  Although those METAR data are known and depicted on the map page, the airport (longpress) does not include them.  This was a 1-line code fix and tested against existing AvareX data (weather.db:{metar,taf}).  See [PR #94](https://github.com/apps4av/avarex/pull/94)
* **Improved plate rendering quality** (cjsindt contribution, see [PR #95](https://github.com/apps4av/avarex/pull/95)).
* **Dynon HDX Support** for missing GDL90 Ownship data; provides "external" GPS support from the Dynon messages broadcast over WiFi.  Otherwise AvareX map/position is largely inop on Dynon HDX ADS-B/WiFi module.  For non-Dynon users this should have no impact.

These are the changes I currently have in my version I've been using for weeks/months, and for expediency are retained here.  I only provide Android and Windows versions since that's what I'm using for development/testing (Windows) and in-flight (Android tablet).

### Android Install
You will have to "side-load" the (latest) .apk from this page.  If that's not something you understand or
are comfortable with, then I can't help you with additional support.  [This information](https://www.apps4av.com/manual-installation.html) from Avare* may help. 

>#### Choosing the right Android ABI File
>To keep the files within Github size limits, there are three versions of the .apk.zip files here.  Choose the version corresponding to your Android device's Application Binary Interface (ABI).  The primary ABIs are `arm64-v8a` (64-bit, most modern devices), `armeabi-v7a` (32-bit, common older devices), and `x86_64` (emulators and some Intel-based devices).

### Feedback/Support
I welcome your feedback on the efficacy of these simple changes.  However, I can offer only limited support at this time.  I am reluctantly making these available due to demand from the forum.  I'm not looking to create a rift in the AvareX community, but these features are desired (per the forum), but not everyone has the time or inclination to tool up with Flutter and make code changes like I have (ong story).  But I'm happy to share what I've been using for months to share/demonstrate the benefits.  I don't expect this to be a long-term situation.  Blue Skies!
