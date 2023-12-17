# pTouch - Cross-platform `touch` replacement written in PHP

This small commandline utility was created to get a better `touch` command for my Windows setup.

It's very tailored and opinionated to my workflow, and as such it will always create files recursively.

## Installation

### General

Download the file, and add it to your `PATH`. 

### Unix

```shell
curl -o ptouch https://raw.githubusercontent.com/caendesilva/ptouch/master/ptouch
chmod +x ptouch
mv ptouch /usr/local/bin
```

If you want it to replace the standard `touch` command, change the filename from `ptouch` to `touch`.


### Windows

On Windows, you'll need to create a Batch alias. Obviously, replace the script path with your own.

```batch
@php C:\Users\User\Documents\WindowsPowerShell\Scripts\ptouch %*
```

Next, you may want to add an alias to your PowerShell profile.

```powershell
Set-Alias -Name touch -Value "C:\Users\User\Documents\WindowsPowerShell\Scripts\ptouch.bat"
```

## Usage

Run the `ptouch` command, followed by the file(s) you want to create.

```bash
ptouch foo.txt foo/bar.md
```

You can also supply `-v` or `--verbose` to get verbose output.

## License

The MIT License.
