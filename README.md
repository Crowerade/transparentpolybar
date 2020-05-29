# Transparent Polybar
![Screenshot 1](https://github.com/Crowerade/transparentpolybar/blob/master/Screenshots/Screenshot%20from%202020-05-29%2014-51-36.png)
![screenshot 2](https://github.com/Crowerade/transparentpolybar/blob/master/Screenshots/Screenshot%20from%202020-05-29%2014-52-33.png)
![screenshot 3](https://github.com/Crowerade/transparentpolybar/blob/master/Screenshots/Screenshot%20from%202020-05-29%2014-55-31.png)
![screenshot 4](https://github.com/Crowerade/transparentpolybar/blob/master/Screenshots/Screenshot%20from%202020-05-29%2014-57-42.png)

A config for polybar highly inspired by polybar-1 in [polybar-themes](https://github.com/adi1090x/polybar-themes).

## Warning
This config was mainly created by [Aditya Shakya](https://github.com/adi1090x), all I did was modifying the first config of his [polybar-themes](https://github.com/adi1090x/polybar-themes). 
Hence, it might be that some files are useless in the repository. If so, you can warn me so that I remove them.

## Installation
For the installation of polybar, refer to the [official repository](https://github.com/polybar/polybar).

Once you have polybar, you can clone the repository in the `.config/polybar` folder in your home directory once you have cleaned it.

```
cd 
cd .config/polybar
git clone https://github.com/Crowerade/transparentpolybar.git
cd transparentpolybar
```
Then, you can execute `launch.sh`, be sure that the file is executable, if not, you can make it executable by typing `chmod +x launch.sh`
```
./launch.sh
```

## Issues
When your have launched your bar, some issues may occur.

### Clicking does not work
They are icons that are clickable : 
- The terminal 🠒 `gnome-terminal`
- The file 🠒 `nautilus`
- The browser 🠒 `firefox`
- The settings 🠒 `gnome-control-center`

These icons should launch the determined software when you click them. If it does not work, then it is most likely that you will have to change the module's settings in `config.ini` by replacing the default software by the one you use.

For instance : You use Chrome instead of Firefox, then you will have to replace `firefox` by `chrome` in the module "browser".

### Offset Workspaces
It is possible that the workspaces are offset and it displays that you are on the first workspace when you are on the second and so one.

For this issue, I have no proper solution to give. Thus I ask to those who are more skilled than I am, if you find a solution then please tell me so that I can adjust the repository.
