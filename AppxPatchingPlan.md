# APPX Patching Plan

- Extract APPX package
- Delete the following file(s):
  * `AppxBlockMap.xml`
  * `AppxSignature.p7x`
  * `[Content_Types].xml`
- Delete the following folder(s):
  * `AppxMetadata/`
- Edit AppxManifest.xml
  * At XML element *"Package/Identity"*, change attribute `Name` from `GAMELOFTSA.Asphalt8Airborne` to `GAMELOFT.Asphalt8Airborne`
  * At XML path *"Package/Applications/Application[Id]" where Id="App"*, delete element `ApplicationContentUriRules`
  * [CONSIDERATION] Change all occurences of `ms-resource:AppName` to `"Asphalt 8: Airborne Classic"`
