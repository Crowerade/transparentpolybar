# Transparent Polybar
![Screenshot 1](https://github.com/Crowerade/transparentpolybar/blob/master/Screenshots/Screenshot%20from%202020-05-29%2014-51-36.png)
![screenshot 2](https://github.com/Crowerade/transparentpolybar/blob/master/Screenshots/Screenshot%20from%202020-05-29%2014-52-33.png)
![screenshot 3](https://github.com/Crowerade/transparentpolybar/blob/master/Screenshots/Screenshot%20from%202020-05-29%2014-55-31.png)
![screenshot 4](https://github.com/Crowerade/transparentpolybar/blob/master/Screenshots/Screenshot%20from%202020-05-29%2014-57-42.png)

Background available [here](https://github.com/LaniJW/linux-pictures/).

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
Then, you can execute `launch.sh`, be sure that the file is executable, if not, you can make it executable by typing <br>
`chmod +x launch.sh`
```
./launch.sh
```

## Usage
![bar](https://github.com/Crowerade/transparentpolybar/blob/master/Screenshots/Bar.png)

The colors are modifiable in `config.ini` and so is the rate of transparency. If you wish to modify the colors and transparancy rates of the menus, you can do so in `scripts/menu` for the small menu on the left, in `scripts/menu_full` for the bigger same menu and in `scripts/sysmenu` for the power menu on the right. What I suggest is that you modify the colors in the first paragraph (in the three files) and then copy paste the first paragraph so that you have the same in the three files. That way, you can have three similar menus.

**We will review each item from left to right.**

On the left, there is the menu, left-click it to display a small menu of all the softwares, right-click it to display the bigger same menu, research is enabled in both cases.

Then you can see your workspaces, if you do not have the right amount of workspaces indicators, you can modify it in the `config.ini` file. The worspaces indicators are clickabe and will lead you to the appointed workspace. It is also possible to scroll with the wheel to change the workspace you are in.

After that, there are 4 icons :
1. The terminal
2. The files manager
3. The browser
4. The settings

The four of them will lead you to the appointed software.

On the right, there is the volume (pulseaudio is used) you can scroll down or up to raise or lower the volume, it is also possible to mute by clicking it.

Then the battery is displayed.

After that we can see the time in 24h format, by clicking it, you can display the date in the following format : <br>
[day of the week abbreviated] [day of the month] [Month] [Year]. Once again, this is modifiable in `config.ini`.

Finally, you can display the power menu by clicking on the final item. Research is enabled.

## Issues
When your have launched your bar, some issues may occur.

### Clicking does not work
There are icons that are clickable : 
- The terminal 🠒 `gnome-terminal`
- The file 🠒 `nautilus`
- The browser 🠒 `firefox`
- The settings 🠒 `gnome-control-center`

These icons should launch the determined software when you click them. If it does not work, then it is most likely that you will have to change the module's settings in `config.ini` by replacing the default software by the one you use.

For instance : You use Chrome instead of Firefox, then you will have to replace `firefox` by `chrome` in the module "browser".

### Offset Workspaces
It is possible that the workspaces indicators are offset and it displays that you are on the first workspace when you are on the second and so on.

For this issue, I have no proper solution to give. Thus I ask to those who are more skilled than I am, if you find a solution then please tell me so that I can adjust the repository.
