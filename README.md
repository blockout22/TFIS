# TFIS

# How To use
1. Create a new plugin and Call it "TFIS_<You_ModName>"
2. Restart your engine
3. In your "TFIS_<You_ModName>", Create a User Widget and change it's parent class to "TFISWidget"
4. (Customize your widget the way you like it)
5. Go back into your oridinal Mod and In side your Buildables Add TFISDescription Component 
6. In the TFISDescription Component details add your TFISWidget to the MoreInfo Array
7. See Below for an example on how your TFIS_<You_ModName>.uplugin file should look
8. Done!

# TFIS_<You_ModName>.Uplugin Example
```
{
	"FileVersion": 3,
	"Version": 1,
	"SemVersion": "1.0.0",
	"VersionName": "1.0",
	"FriendlyName": "TFIS_ItemTeleporter",
	"Description": "",
	"Category": "Other",
	"CreatedBy": "Blockout22",
	"CreatedByURL": "",
	"DocsURL": "",
	"MarketplaceURL": "",
	"SupportURL": "",
	"CanContainContent": true,
	"IsBetaVersion": false,
	"IsExperimentalVersion": false,
	"Installed": false,
	"Plugins": [
		{
			"Enabled": true,
			"Name": "SML",
			"SemVersion": "^3.1.1",
			"bIsOptional": false
		},
		{
			"Enabled": true,
			"Name": "TFIS",
			"SemVersion": "^1.0.1",
			"bIsOptional": false
		}
	]
}
```

# FAQ

### Does my main mod need to depend on TFIS?
Your main mod doesn't need to depend on TFIS but your "TFIS_<You_ModName>" does have to depend on TFIS

### What happend if the user uninstalls TFIS, will my main mod stop working?
No, See above question.
 
