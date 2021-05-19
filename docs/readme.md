# Flutter Desktop App

This project aims to illustrate how to

- Develop Flutter App for desktop (linux) platforms
- Pack a flutter project into an AppImage. 
- Setting up a CI workflow to test and build using Github Actions


## Requirements

- Linux (Tested on Ubuntu >= 18.04 and Debian Buster)
- Flutter (2.2 or higher)
- appimage-builder

## Development


```sh
git clone https://github.com/alphaolomi/flutterapp.git
cd flutterapp
```

```sh
# enable flutter desktop support
flutter channel dev
flutter upgrade
flutter config --enable-linux-desktop
```

### Run locally

```sh
# Run the flutter app
flutter run -d linux
```
### Build for linux 
```sh
# build the flutter app
flutter build linux
```

```sh
# build the AppImage
appimage-builder --skip-test
```


## Ref

- https://flutter.dev/desktop