### Download a file to an existing folder with CURL

#### Command

```
curl -LO https://github.com/vot/ffbinaries-prebuilt/releases/download/v4.2.1/ffmpeg-4.2.1-win-32.zip --output-dir runtimes/win10-x86/native -s
```

#### Output

Downloads `ffmpeg-4.2.1-win-32.zip` to an existing folder `runtimes/win10-x86/native`

#### Details
`-L` follow the redirects

`-O` indicate the file location

`--output-dir` indicate the folder location relative to the one where this command is executed

`-s` silent run

#### Extra options
If the folder doesn't exist, `--create-dirs` could be used

#### Alternative

Download without creating the directory structure first

```
curl -o runtimes/linux-x32/native/ffmpeg-4.2.1-linux-32.zip --create-dirs -LO https://github.com/vot/ffbinaries-prebuilt/releases/download/v4.2.1/ffmpeg-4.2.1-linux-32.zip -s
```

#### Details
`-L` follow the redirects

`-O` indicate the file location

`-o` indicate the folder location of the file to be download and the file name

`-s` silent run
