# embi-manifest
This repository provides manifests for Embi OS yocto builds

## How to use this layer

Using this layer requires Google's repo tool to be installed, you can download it with:
```bash
curl https://storage.googleapis.com/git-repo-downloads/repo > ~/.local/bin/repo
chmod a+rx ~/.local/bin/repo
```

After installing the repo tool, run following commands to initialize the build environment.
```bash
repo init -u git://github.com:Romain-Donze/embi-manifest -m <manifest>
repo sync

export MACHINE=raspberrypi4-64 && source ./setup-environment.sh
```

For more information about Boot to Qt, see https://doc.qt.io/QtForDeviceCreation/

