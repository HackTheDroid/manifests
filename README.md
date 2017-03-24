LineageOS
===========

HTC HD2 Build
------------------
    branch: cm-12.1_leo
    repo init -u ssh://mygit/media/aosp-mirror/github/shugaoye/manifests -b cm-12.1_leo

20170324: Changed kernel to android_kernel_htcleo-2.6.32.
20170323: Changed to mygit.
20170322: Build TWRP for device/htc/leo.
20170321: Use GitHub for the changes.
          maniacx/android_kernel_htcleo-3.0_older - cm-12.1
          maniacx/android_device_htc_leo - cm-12.1
          maniacx/android_hardware_qcom_display - cm-12.1_leo
          maniacx/android_hardware_qcom_media-legacy -  cm-12.1-caf-qsd8k
          maniacx/android_hardware_qcom_audio - cm-12.1-caf-qsd8k

Submitting Patches
------------------
Patches are always welcome!  Please submit your patches via LineageOS Gerrit!
You can do this by using these commands:

    (From root android directory)
    . build/envsetup.sh
    (Go to repo you are patching, make your changes and commit)
    cmgerrit <for(new)/changes(patch set)> <branch/change-id> 

    repo start cm-11.0 .
    (Make your changes and commit)
    repo upload .
Note: "." meaning current directory
For more help on using this tool, use this command: repo help upload

Make your changes and commit with a detailed message, starting with what you are working with (i.e. vision: Update Kernel)
Commit your patches in a single commit. Squash multiple commit using this command: git rebase -i HEAD~<# of commits>

To view the status of your and others' patches, visit [LineageOS Code Review](http://review.lineageos.org/)


Getting Started
---------------

To get started with Android/LineageOS, you'll need to get
familiar with [Git and Repo](http://source.android.com/source/using-repo.html).

To initialize your local repository using the LineageOS trees, use a command like this:

    repo init -u git://github.com/LineageOS/android.git -b cm-11.0

Then to sync up:

    repo sync

Please see the [LineageOS Wiki](http://wiki.lineageos.org/) for building instructions.

For more information on this Github Organization and how it is structured, 
please [read the wiki article](http://wiki.lineageos.org/w/Github_Organization)

Buildbot
--------

All supported devices are built nightly and periodically as changes are committed to ensure the source trees remain buildable.

You can view the current build statuses at [LineageOS Jenkins](http://jenkins.lineageos.org/)

