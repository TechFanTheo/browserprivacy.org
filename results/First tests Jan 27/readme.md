For now this is manual results using  https://privacytests.org/me.html. It isn't yet regrouped and is per browser only with some categories missing. using  Linux, I couldn't suceed running the tests. Not knowing Javascript doesn't help. Plus Arthur code has compatibility issues with Linux as it is designed for Mac. For a very rough to read overview of the challenges I faced you can read https://monograph.notesnook.com/65b20432aeaeae1c343e3e40.

Below is rules for hardening
(Most sites should work. JS on for secure sites)

Chrome :
Has a "Privacy Review" journey to quickly review privacy settings. However when disabling third-party cookies, it will still allow sites to share with groupped sites. Youtube.com can say it wants to share cookies with Google.com for example. I hadn't seen this, but now is disabled. Allow- Chrome Sign-in disabled. Enhanced protection on.

vivaldi:
Select Tracker and Ads blocking on start-up. Block Third-Parties cookies. Form-Autofill Assist disabled and other auto-fill also disabled.Disable Hangouts (for Google Meet) extension. Disabled IP broadcast for WebRTC.Unfortunately, Vivaldi has some very specific fonts. This might be fetched from system. Enables FP. (might investigate in future). Disable Feeds recognition. Disable DirectMatch (affiliation links related).Disable passwod saving at vivaldi://password-manager/settings. For Cookies, SessionOnly means it will clear them after logout, so you can't stay logged in. Since there isn't a per-site exception keep cookies on. Vivaldi very good visualisation of cookies dat so you can delete those of untrutsed sites.Manually remove homescreen sponsored links.
