appimage-builder-flutter-example
This project aims to ilustrate how to pack a flutter project into an AppImage. Also, includes instructions for setting un a CI workflow using Github Actions.

Requirementes
Ubuntu (18.04 or higher)
flutter
appimage-builder
Build
git clone https://github.com/AppImageCrafters/appimage-builder-flutter-example.git
cd appimage-builder-flutter-example

# enable flutter desktop support
flutter channel dev
flutter upgrade
flutter config --enable-linux-desktop

# build the flutter app
flutter build linux

# build the AppImage
appimage-builder --skip-test