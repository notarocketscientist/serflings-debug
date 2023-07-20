# Run Serflings with Wine (Ubuntu 20.04.6 LTS)

## Wine from "default" repos

Install Wine - currently version 5.0-3ubuntu1 from 2020 (?):

```
sudo apt install wine
```

Download latest stable Serflings version (2.0 - with bundled JRE) and run the game:

```
cd <game dir>
wine serflings.exe
```

### Testing

So far, this has been testet/noticed:

* game launches
* right-click scrolling is a bit to fast (maybe a Wine setting?)
* tick and render times look "normal" to me: around 50 FPS and 5 ms render time

## Latest Wine from Wine repos

This will install current stable version 8.0.2 of Wine.

Installation how-to from: https://wiki.winehq.org/Ubuntu


```
sudo dpkg --add-architecture i386 
sudo mkdir -pm755 /etc/apt/keyrings
sudo wget -O /etc/apt/keyrings/winehq-archive.key https://dl.winehq.org/wine-builds/winehq.key
sudo wget -NP /etc/apt/sources.list.d/ https://dl.winehq.org/wine-builds/ubuntu/dists/focal/winehq-focal.sources
sudo apt update
sudo apt install --install-recommends winehq-stable
```

Download latest stable Serflings version (2.0 - with bundled JRE) and run the game:

```
cd <game dir>
wine serflings.exe
```

Mono:

```
At first launch, Wine wants to install "wine-mono" package. Choose `Yes, install`.
```

### Testing

So far, this has been testet/noticed:

* game launches
* right-click scrolling is a bit to fast (maybe a Wine setting?)
* tick and render times look "normal" to me: around 50 FPS and 5 ms render time