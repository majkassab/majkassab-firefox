This configuration will improve the security of Firefox

1- open firefox

2- In the address bar, type about:config and press Return

3-Seach and edit the following settings:

=========== Level 1 - Comfortable Protection ===========

security.pki.distrust_ca_policy;2

security.tls.version.min;3

security.tls.version.max;4

security.mixed_content.block_display_content;true

security.mixed_content.block_object_subrequest;true

security.ssl.require_safe_negotiation true

security.webauth.u2f;true

network.trr.mode 2

network.trr.uri;https://mozilla.cloudflare-dns.com/dns-query

network.trr.bootstrapAddress;1.1.1.1

network.security.esni.enabled;true

network.IDN_show_punycode;true

=========== Level 2 - High Protection ===========

security.ssl3.rsa_des_ede3_sha;false

security.ssl3.rsa_aes_128_sha;false

security.ssl3.rsa_aes_256_sha;false

security.OCSP.require;true

security.ssl.treat_unsafe_negotiation_as_broken;true

dom.battery.enabled;false

extensions.pocket.enabled;false

privacy.resistFingerprinting;true

privacy.firstparty.isolate;true

privacy.trackingprotection.fingerprinting.enabled;true

privacy.trackingprotection.cryptomining.enabled;true

webgl.disabled;true

browser.cache.offline.enable;false

browser.safebrowsing.malware.enabled;false

browser.safebrowsing.phishing.enabled;false

=========== Level 3 - Paranoid Protection ===========

dom.event.clipboardevents.enabled;false

dom.serviceWorkers.enabled;false //about:serviceworkers

media.peerconnection.enabled;false

media.navigator.enabled;false

privacy.firstparty.isolate.restrict_opener_access=false

dom.battery.enabled;false

network.cookie.lifetimePolicy;2

network.http.referer.trimmingPolicy;2

network.http.referer.XOriginPolicy;2

network.http.referer.XOriginTrimmingPolicy;2

browser.sessionstore.privacy_level;2

geo.enabled;false
