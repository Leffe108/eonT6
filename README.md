#eonT6
A dice emulator for the RPG Eon

Everything is in one file on purpous.

Just open eonT6.html or eomT6iv.html with your favourite browser.
The program works without internet. 

The only difference between eonT6.html and eonT6iv.html is the background image. I get the image by linking to helmgast.se, therefore the picture will dissapear if you do not have internet acces, or if Helmgast removes it. But every thing else will continue to work as before.

eonT6.html will always look the same, unless you edit it yourself. 
(Or if you change browser, difterent browsers may give slightly different appearance. Or if you change screen or screen setting, this might affect colurs and brightness.)

## Some kind of manual
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
