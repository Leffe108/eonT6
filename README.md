#eonT6 cordova
eonT6 is a dice emulator for the RPG Eon.

This is a fork of eonT that has transformed eonT6.html into a Cordova app. Original eonT6.html has been renamed to www/index.html and additional cordova project files have been added.

## Original eonT6 manual
You can enter ether numbers or equations as "Number of T6" and "Extra". If your your "Extra" is less then 0 or more than 3, this program will re calculate the number of dices according to Eon rules.
As an example, if you enter:

|**Number of T6:** | **3+2**|
|---               | ---    |
|**Extra:**        | **-1** |

This will be recalculated:

**( 3+2 ) T6 + ( -1 ) = 4 T6 + 3**

This program will always do ob-rolles acoring to Eon rules. This means that if the outcome of a dice is 6, this will not be counted, but instead two new dices are rolled.

All dices are displayed.

All results, inkluding the one you just rolled, are shown in a list at the botom of the page. Update the borowser to empty this list.

## Building Cordova app (Android, iPhone etc)

Make sure you have the native toolchain for the platform you like to compile for. Also make sure you have cordova CLI installed in PATH. Building for iPhone requires a Mac and that you sign up for Apple developer program and pay their yearly fee.

```
> cordova platform add android
> cordova build android
# Attach your phone to your computer via cable (or make sure you have an emulator set up)
> cordova run android
```

Replace 'android' with 'ios' if you want to build for iPhone.
