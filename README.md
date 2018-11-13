Overview
=======

Nusantara Recovery is a Recovery Project developed by the Nusantara Devs Team from Indonesia, Nusantara Recovery is a derivative of Official TWRP that has been modified by the developer for the purpose of completing the features and uniqueness of the user interface. We  prioritize the features and stability contained in this recovery. Why is it called Nusantara Recovery? Because Nusantara in Indonesia means from Sabang to Merauke, meaning that one nation of one nation is one language, all are the same, there is no difference, that is Indonesia.

Features
=======

* In development
    
Changelog
=======    

~ Alpha ~
* In development

Credits
=======
* [**TEAMWIN RECOVERY PROJECT (BASE)**](https://github.com/TeamWin)
* [**OMNIROM**](https://github.com/omnirom)
* [**REDWOLF RECOVERY PROJECT**](https://github.com/RedWolfRecovery)
* [**PITCHBLACK RECOVERY PROJECT**](https://github.com/PitchBlack-Recovery)
* [**DARK RECOVERY PROJECT**](https://github.com/DarkRecovery)
* [**ORANGEFOX RECOVERY PROJECT**](https://gitlab.com/OrangeFox)
* [**BATIK RECOVERY PROJECT**](https://github.com/BatikRecovery)

Getting Started
===============

To get started with OMNI sources to build TWRP, you'll need to get
familiar with [Git and Repo](https://source.android.com/source/using-repo.html).

Make Directory 

```bash
     mkdir <source-dir>
     cd <source-dir>
```

(For Example : nusrec)

```bash
     mkdir ~/nusrec
     cd ~/nusrec
```

To initialize Nusantara Recovery local repository, use this command :
```bash
    repo init -u git://github.com/NusantaraRecovery/nr_manifest.git -b nr
```

To initialize a shallow clone, which will save even more space, use a command like this:
```bash
    repo init --depth=1 -u git://github.com/NusantaraRecovery/nr_manifest.git -b nr
```

Then to sync up :
```bash
    repo sync -j8
```

 Clone Device Tree Of Nusantara Recovery
=============================

Ceck on https://github.com/BatikRecovery/br_devices for your device

Example :

```bash
    git clone https://github.com/NusantaraRecovery/nr_devices.git -b land device/xiaomi/land
```

 Compilation Of Nusantara Recovery
=============================
 
```bash
     cd <source-dir>
     export ALLOW_MISSING_DEPENDENCIES=true
     . build/envsetup.sh
```     
     
Change Maintainer
```bash
     export NR_MAINTAINER="your-name"
```
 
```bash
     lunch omni_<device>-eng
     mka recoveryimage
```

If it fails to compile
```bash
     export LC_ALL=C
```
