For now this is manual results using  https://privacytests.org/me.html. It isn't yet regrouped and is per browser only with some categories missing. using  Linux, I couldn't suceed running the tests. Not knowing Javascript doesn't help. Plus Arthur code has compatibility issues with Linux as it is designed for Mac. For a very rough to read overview of the challenges I faced you can read https://monograph.notesnook.com/65b20432aeaeae1c343e3e40.
The tests are run on Linux Ubuntu 23.10

Below is rules for hardening
(Most sites should work. JS on for secure sites)

Chrome :
Has a "Privacy Review" journey to quickly review privacy settings. However when disabling third-party cookies, it will still allow sites to share with groupped sites. Youtube.com can say it wants to share cookies with Google.com for example. I hadn't seen this, but now is disabled. Allow- Chrome Sign-in disabled. Enhanced protection on.

vivaldi:
Select Tracker and Ads blocking on start-up. Block Third-Parties cookies. Form-Autofill Assist disabled and other auto-fill also disabled.Disable Hangouts (for Google Meet) extension. Disabled IP broadcast for WebRTC.Unfortunately, Vivaldi has some very specific fonts. This might be fetched from system. Enables FP. (might investigate in future). Disable Feeds recognition. Disable DirectMatch (affiliation links related).Disable passwod saving at vivaldi://password-manager/settings. For Cookies, SessionOnly means it will clear them after logout, so you can't stay logged in. Since there isn't a per-site exception keep cookies on*. Vivaldi very good visualisation of cookies dat so you can delete those of untrutsed sites.Manually remove homescreen sponsored links. Change search engine to DuckDuckGo. Let Do Not Track be disabled. DNT isn't used by most so this make you stand-out and many websites don't answer it. Not sure about this one but put date and time format to follow the language.Enable Always Use Secure Connection. Disable widevine, although it doesnt seem to even disable it lol.
*Edit: Put Cookies on session-only. For sites you want to log into, you can allow them to save data on device by clicking on the lock icon and then cookies and then manage site data. Click on the dot and allow save data.
Put Startpage to vivaldi://startpage instead of vivaldi.com. Did not disable hyperlink audit blocking as only Firefox-based do it and is very niche.

Mullvad browser : Hardened is Safe Mode. Didn't modify uBlock and NoScript settings (those are the two default extensions). In second edition, WebRTC will be disabled, as it can leak IP on video calls due to Mozilla bug. See https://gitlab.torproject.org/tpo/applications/mullvad-browser/-/issues/151

Tor Browser :
Enable Safe Mode as JS must stay on. Didn't enable Malware protection as it can make you more fingerprintable. See https://tor.stackexchange.com/questions/22024/how-does-tor-browser-protect-against-fraudulent-pages. 

Brave :
Followed PrivacyGuides Hardening. Interrestingly I had to refresh the test page twice when running on hardened brave.If I didn't the test was just stuck.

Firefox : followed Privacy Guide. Plus Duckduckgo as search engine. Disabled Sponsored Shortcuts.