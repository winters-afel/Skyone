# Skyone
SkyOne Sports
PROCEDURE TO DEPLOY NEW APPLICATION
1.	Duplicate parent project and rename with new name
2.	Change package name
a.	Change in the android > app > src > debug > AndroidManifest.xml
b.	Change in the android > app > src > main > AndroidManifest.xml
c.	Change in the android > app > src > profile > AndroidManifest.xml

3.	Rename App Name in android > app > src > profile > AndroidManifest.xml
4.	Change folder name related to package path in android > app > src > main > java > com > project > [CHANGE NAME]
5.	Change package name in MainActivity inside src > main > java > [package path]
6.	Change AppIcon for both android (mipmap folders) and ios (Assets.xcassets folder)
a.	Upload logo on this site (https://appicon.co/)
b.	Then generate appicon for both android and iOS
c.	Replace all mipmap folders for android with new one from location android > app > src > main > res
d.	Replace Assets.xcassets folder with new one from ios > runner
7.	 Change startup Icon in android > app > src > main > res > drawable
8.	Change google-services.json file
a.	Generate new file from firebase console if file not exists
b.	Open link (https://console.firebase.google.com/)
c.	Paste file in location android > app
9.	Update AndroidManifest android > app > src > main > AndroidManifest.xml
a.	Change Admob App ID (if applied for ads)
b.	Change deeplink url
i.	Generate deeplink url if not exits
10.	Update both build.grade files (android > app > build.grade)
11.	Update key.properties file
12.	Update pubspec.yaml
13.	Update api.dart
14.	Update global.dart
15.	Change/Set ad units on the dashboard
16.	Block some country from view livestream
17.	Register Country in PremiumCountryUserAdmin where their users are not allowed to watch ads
18.	Block some country from using app at all in BlockListedIsoCodeFromUsingTheApp
19.	Test share links
