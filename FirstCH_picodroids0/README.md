 # First flag

I've used jadx to decompile the `zero.apk` file to review the source code:
![Alt text](CH1_image.png)

Going trough the files, we take a look at MainActivity and we find _buttonClick_ calling _getFlag_ method from FlagstaffHill class:
![Alt text](CH1_image1.png)

The _getFlag_ function captures and logs the result of invoking a native method from the JNI library, using the given input as its argument.
![Alt text](CH1_iamge2.png)

I've used an android emulator in order to run the app
![Alt text](CH1_image3.png)

After that I've looked into the logs searching for **pico**, reavealing the flag.
![Alt text](CH1_image4.png)

**picoCTF{a.moose.once.bit.my.sister}**

