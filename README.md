
## 앱 빌드 환경 설정

- [NodeJS LTS](https://nodejs.org/ko/) : 12 버전 선택
- Cocoapods
  - intel chip
    ```bash
    sudo gem install cocoapods
    ```
  - m1
    1. [install homebrew](https://docs.brew.sh/Installation)
    2. terminal
    ```bash
    eval $(/opt/homebrew/bin/brew shellenv)

    brew install cocoapods
    ```
- [XCode Download](https://developer.apple.com/xcode/)
- XCode Setting
  - Xcode command line tools
    **Xcode → Preferences → Locations** 
    드롭다운 마지막 버전 선택
  - Xcode login
    **Xcode → Preferences...→ Accounts → Apple IDs**
  - terminal
    ```bash
    sudo xcode-select --install

    sudo xcode-select -s ${your_xcode_path}/Xcode.app/Contents/Developer
    ```
- [Java Download](https://www.oracle.com/java/technologies/downloads/#jdk17-mac)
- [Android Studio Download](https://developer.android.com/studio)
- Android Studio Setting
  - Android Studio→Preferences→Apprearances & Behavior→System Settings→Android SDK
    - 체크 박스 선택
    - Android SDK Build-Tools
    - Android SDK Command-line Tools
    - Android Emulator
    - Android SDK Platform-Tools
- Typescript Install
  ```bash
  sudo npm install -g typescript
  ```
- Custom Module Build
  ```bash
  cd ${your_repo}/giftistar-custom-module

  npm run build_custom_module
  ```
- npm install
- npx cap sync

## 안드로이드 빌드

npm run local-android

## 아이폰 빌드

npm run local-ios
