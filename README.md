# notiePlusPlus
NotiePlusPlus is a much superior version of [jaredreich's notie](https://github.com/jaredreich/notie), featuring both far smaller file sizes and a much more convienent single-file delivery that improves load speed. I decided to make a whole new repoitory instead of submitting this as a pull request because this repository makes several huge changes that I believe jaredreich would not understand as improvements because these changes would super-seed all other pull requests due to the entire file structure changing.

1. Webpack -> Closure Compiler. The Webpack system that jaredreich uses super-massively bloats the file size.
2. CSS and JS loaded separately -> All loaded together as one JS file. There is an easy `async=""` attribute for scripts, but no such convenient option for stylesheets (aside from `lazload=""`, but `lazyload=""` only works in Internet Explorer and Edge). Thus, a single asynchronous script will have less impact on load speed than with the addition of a synchronous stylesheet.
3. cdnjs -> Dropbox. This is more of a disadvantage. This library does not have enough stars to be hosted on cdnjs.

If you are jaredreich, and you actually wish to merge my changes with your original notie repository, then please copy over the files as you see fit, open an issue at this repository that you are merging the changes with your repository, and I shall close this repository promptly. Until then, this repository will stay open to provide developers with a better alternative.
