# Blog

This repository is the source for my github pages, also my blog.  
The structure is from Jekyll pages. I wrote the CSS and JS files myself.

## If you are trying Jekyll for your .github.io , a word....

*Quick and easy blog pages?*  
- *Use [Jekyll](https://github.com/jekyll/jekyll) with defaults and add a theme.*

*Quick, easy and also lazy?*  
- *Try [fast-template](https://github.com/fastai/fast_template) and generate pages with very less work.*

*Easy and Good looking?*
- *Use [Beautiful Jekyll](https://github.com/daattali/beautiful-jekyll).*

### Most important part

I decided to use my own CSS and JS, just so that I could explore the stuff. However, since Jekyll structure is based on liquids we cannot test our blog pages locally in usual manner. It requires jekyll software on your device.

I use Arch Linux. The pacman ruby version is different from that of requirements for Jekyll. Besides we need appropriate versions of Jekyll, Ruby gems and bundler. Generating Ruby from source file becomes a tedious task.  

The process is quite simple on Windows.  
The stable version that Ruby Installer (for windows) offers is `v2.7.3-1` which is compatible with github-pages. All you have to do is:

- Go to [Ruby Installer Downloads](https://rubyinstaller.org/downloads/) and download the .exe file for stable version with devkit.

- After installation, open command prompt or powershell and run `gem install github-pages` and then `bundler install`

- Now you are ready to test the site locally, `cd` to your blog directory and run `bundler exec jekyll serve --watch`. You can use your browser and test the site at [http://127.0.0.1:4000/](http://127.0.0.1:4000/)

- If it doesn't work, it is probably because running `gem install github-pages` did not install all required gems. Check the error report and run `gem install _gem_name_`.
