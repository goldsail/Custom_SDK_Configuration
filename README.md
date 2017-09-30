# How to configure GLXSS Pro SDK on Android Studio 

## Step 1: Unzip files

- Unzip ```android-sdk_user.build_windows.zip```. Assume the unzipped SDK folder is in path ```PathA/GlxssProSDK```, which contains several folders, e.g. ```platforms``` and ```platform-tools```. 

- Unzip ```GLXSS_API_TEST_src.zip```. Assume the unzipped source folder is in path ```PathB/GLXSS_API_TEST_src```. 

## Step 2: Import the non-gradle project into Android Studio with Gradle

- Open Android Studio, exit the current project, and click "Import project (Eclipse ADT, Gradle, etc.)" on your right. 

- Select path ```PathB/GLXSS_API_TEST_src``` and continue. 

- Specify another destination path to store the imported project. Here I use ```PathB/GLXSS_API_TEST``` for example. 

- Finish the import wizzard with all other options set default.

## Step 3: Configure SDK paths and API levels. 

- Do not update Gradle in case of no downward compatibility. ![](https://i.loli.net/2017/09/30/59cf7695a5454.png)

- In ```File -> Project Structure```, set the SDK path to ```PathA/GlxssProSDK``` and JDK path to embedded. ![](https://i.loli.net/2017/09/30/59cf779a6e27f.png)

- Set API level and Build Tools version as follows. ![](https://i.loli.net/2017/09/30/59cf775a72222.png)

## Step 4: Install support repositories

- In the SDK Manager, install ```Android Support Repositories``` ![](https://i.loli.net/2017/09/30/59cf77f01f36d.png)

## Step 5: Refresh and build

- Make Project in ```Build``` menu. 

- Build APK ```Build``` menu. 
