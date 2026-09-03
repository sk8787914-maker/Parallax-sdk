# Parallax SDK

The complete Android SDK source, including the Twitter/X and Facebook OAuth
compatibility fixes, is in [`BLACK-OPEN/`](BLACK-OPEN/). The Gradle module is
[`BLACK-OPEN/RIYAZ-VIP`](BLACK-OPEN/RIYAZ-VIP) and is published as the
`ParallaxCore` project.

## Build locally

```bash
cd BLACK-OPEN
./gradlew :ParallaxCore:assembleRelease
```

The release AAR is written to
`RIYAZ-VIP/build/outputs/aar/`.

## CI and releases

GitHub Actions builds the release AAR and runs unit tests for pull requests and
pushes to `main`. The AAR is uploaded as a workflow artifact. Pushing a version
tag such as `v2.0.0` also creates a GitHub Release and attaches the generated
AAR.
