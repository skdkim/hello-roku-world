# hello-roku-world

## How to zip properly to avoid upload Error
### Main Error: 'Install Failure: No manifest. Invalid package.'

The reason why you're getting this error is because you want to zip the contents of the folder, not the parent folder itself.

You can do this 2 ways, through cmd or with gui.

### cmd
1. Navigate to the root level of your directory
2. zip -r ../hello-world.zip .

zip => the command
-r => will recurse into directories
../hello-world.zip => creates the name of the file and saves it outside of the current directory
. => represents current folder

### gui
You have less control over what certain aspects of the zip process but it's easy enough to fix
1. Navigate to the root level of your directory
2. Highlight all the contents of the directory
3. Right click and choose the option: Compress # Items

Your zipped folder will appear inside that directory and most likely be names Archive.zip
