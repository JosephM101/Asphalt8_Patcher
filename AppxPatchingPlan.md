# APPX Patching Plan

- Extract APPX package
- Delete the following file(s):
  * `AppxBlockMap.xml`
  * `AppxSignature.p7x`
  * `[Content_Types].xml`
- Delete the following folder(s):
  * `AppxMetadata/`
- Edit AppxManifest.xml
    * At XML path *"Package/Identity"*, change attribute `Name` to `GAMELOFT.Asphalt8Airborne`
  * At XML path *"Package/Applications/Application[0]"*, remove entry `"ApplicationContentUriRules"`