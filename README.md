Role Name
=========

An Ansible role to install the Android NDK.


Dependencies
------------
Oracle Java

Role Variables
--------------
- `android_ndk_cache_dir`: (default: `/tmp/ansible-cache`) Cache folder for downloads
- `android_ndk_cache_dir`: (default: `12`) SDK version to download
- `android_ndk_zipfile`: (default: `android-ndk-r{{android_ndk_version}}-linux-x86_64.zip`) - Zip file to download
- `android_ndk_folder`:  (default: `android-ndk-r{{android_ndk_version}}`) - Folder to extract the SDK to


Example Playbook
----------------
    - hosts: servers
      roles:
         - { role: munkyjunky.android-ndk }


License
-------
MIT
