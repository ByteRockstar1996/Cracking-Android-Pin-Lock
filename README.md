# Cracking-Android-Pin-Lock
Python script to brute force Android Pin Lock on android version pre 4.4

Needed to hav adb access to a rooted android device.

Need to 'adb pull /data/data/com.android.providers.setings/databases/settings.db'

This has password salt stored

Then 'adb pull /data/system/password.key'

This has MD5 & SHA1 hashes stored

Finally need to 'adb pull /data/system/device_policies.xml'

This will tell you PIN length. Also if the lock type is a passsword it will tell you length and make up of the password 

Then run the script with these files in the same folder and it will crack the password.
