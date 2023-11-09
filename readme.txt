*********Main note 0.1 - Only use expo on ios at first to eject and build android studio simulator version. (run these commands from root react native project terminal on ios device, not windows, linux, chromebook, etc)

a.1 (make sure to run npx expo prebuild on ios device after cloning repo from github/git or download from google drive, then run below commands from root react native project terminal)

npm i yarn && yarn add expo

a2:
npx expo prebuild && npx expo start

b. open android innermost folder in android studio (after running npx expo start)
Click on the green run arrow/button in android studio (simulator should start with app running)

c. update native android code if needed, otherwise continue to build main app in react native, and test from react native project terminal with:

npx expo start
(press w for web)


**Main note 0.25 - To resolve common errors and confirm android/gradle is setup correctly (send result to chatgpt):

cd android
./gradlew assembleDebug

OR

cd android
./gradlew assembleDebug --stacktrace
