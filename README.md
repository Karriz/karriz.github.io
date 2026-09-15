# karriz.github.io

This user site hosts origin-level configuration for
[Katu Maps](https://karriz.github.io/Katu-Maps/).

## Android Digital Asset Links

`.well-known/assetlinks.json` associates the origin with the Android app
`io.github.karriz.katumaps`. It contains the local upload-key certificate for
locally signed builds, the Play signing certificate observed on the generated
universal APK for pre-Android-17 devices, and the classical and post-quantum
Android 17+ certificate fingerprints supplied by Play Console. Certificate
fingerprints are public metadata; passwords and private keys must never be
committed.

After changes deploy, verify:

```text
https://karriz.github.io/.well-known/assetlinks.json
```
