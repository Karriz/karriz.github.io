# karriz.github.io

This user site hosts origin-level configuration for
[Katu Maps](https://karriz.github.io/Katu-Maps/).

## Android Digital Asset Links

`.well-known/assetlinks.json` associates the origin with the Android app
`io.github.karriz.katumaps`. The initial entry contains the local upload-key
certificate fingerprint, enabling verification of locally signed builds.

Before releasing through Google Play, add the **App signing key certificate**
SHA-256 fingerprint from Play Console → Setup → App integrity to the
`sha256_cert_fingerprints` array. Do not replace the existing upload-key
fingerprint if local-build verification is still needed. The Play app-signing
fingerprint is public certificate metadata, not a password or private key.

After changes deploy, verify:

```text
https://karriz.github.io/.well-known/assetlinks.json
```
