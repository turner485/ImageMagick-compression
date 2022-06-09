# Image Compression w/ ImageMagick

## Installation

1. From [this page](https://imagemagick.org/script/download.php#windows) download and install ‘ImageMagick-7.0.10-34-Q16-HDRI-x64-dll.exe’
1. During setup, make sure the legacy covert tick box is checked and application directory is added to system path
1. After installation, check that it’s in the location ‘C:\Program Files\ImageMagick-7.0.10-Q16-HDRI’
1. Create a system variable with ‘C:\Program Files\ImageMagick-7.0.10-Q16-HDRI\convert’ as the path. Call the variable ‘magick’
1. Open your terminal and check the variable works
1. In the root of the repo, create a file called `repo-config` (note: no file extension) and copy/paste the code block below into it
1. Run the bash script

**‘repo-config’ code:**

```bash
magick=magick
ask_webp=true
```

## Things to know

- When copying file paths, you need to make sure there are no spaces otherwise it’ll break when pasting
- To prevent the script asking if you want webp conversion, replace `ask_webp=true` with `ask_webp=false` in the ‘repo-config’ file
- The user is asked to create a config file during installation so they can configure the script to suit their needs without affecting the tracked files (because of the .gitignore file)
