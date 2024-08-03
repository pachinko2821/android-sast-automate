# Android SAST Automate
Decompiling large APK's is often extremely slow on when on desktop. This repository has a workflow that decompiles the pushed APK file, and uploads the files as an artifact.

To use this workflow run the following commands:

```sh
# Fork the repository and clone it on your machine.
git clone git@github.com:your-github-username/android-sast-automate.git

# Delete the existing apk
git rm vrt_merged.apk

# Add your own APK
git add your-apk-file.apk
git commit -m "switch apk file"
git push
```

Decompilation should now begin on a github runner, which is significantly faster. The decompiled files are uploaded as an artificat that you can download.

# TO-DO
- Add automated SAST scanning on decompiled files.