# Settings Saver

This library allows you to store the settings of your application. It uses serializng at XML format. You should create a simple class with public fields and pass it into a SettingsSaver class.

## How to use:


```
SettingsSaver.Saver<Your_Settings_Class> settingsSaver = 
   new SettingsSaver.Saver<Your_Settings_Class>();

Settings sets = settingsSaver.Activate("Your_Project_Name");

//some code

settingsSaver.Save();
```


Also you can use a Reset() function to delete settings file and reset settings to default values:


```
settingsSaver.Reset();
```



	This code is listed under the Creative Commons Attribution-ShareAlike license.
	You may use, redistribute, remix, tweak, and build upon this work non-commercially and commercially,
	as long as you credit the author by linking back and license your new creations under the same terms.
	This code is provided 'as is'. Author disclaims any implied warranty.
	Zuev Aleksandr, 2024, all rights reserved.