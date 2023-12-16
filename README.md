# pTouch - Cross-platform `touch` replacement written in PHP

This small commandline utility was created to get a better `touch` command for my Windows setup.

It's very tailored and opinionated to my workflow, and as such it will always create files recursively.

## Installation

Download the file, and add it to your `PATH.` On Windows, you'll need to create a Batch alias.

If you want it to replace the standard `touch` command, change the filename from `ptouch` to `touch`.

## Usage

Run the `ptouch` command, followed by the file(s) you want to create.

```bash
ptouch foo.txt foo/bar.md
```

## License

The MIT License.
