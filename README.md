# Video-wallpapers

Inside the `./videos` directory there are a bunch of small videos usable as wallpaper with the help of [this script](/videos/wallset).

All you have to do is position yourself inside `./videos` and run `wallset --video <whatever.mp4>`; viceversa, to halt your video-wallpaper, just `wallset --quit`.


### Order!

With the intent of keeping the repo in order, I wrote a simple script that renames every file inside it with a progresive number: just throw any gif inside `./videos` and run `./vid-rename`: it will convert all the gif files inside the direcory in an mp4 before rename it appropriately. This is becouse on the web is much easier to find gifs than small videos.

---

To speed things up, you can add these two functions in your `~/.zshrc` (or `~/.bashrc`) too:

```
function wallvideo () { wallset --video $1 ; }
function wallquit () { wallset --quit ; }
```
