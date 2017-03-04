# yarr-fish-function

> An alias of `yarn run` with completion for [Fish](http://fishshell.com/) shell.

## Script description

It is possible to specify a description of a script by adding a shell comment at
the end of the script in your `package.json`:
```json
{
  "scripts": {
    "clean": "rm -rf dist/ # Clean the project",
    "build": "node scripts/build # Build the project",
    "publish": "node publish",
  }
}
```

Which will give for completion:
```sh
$ yarr
build      (Build the project)
clean      (Clean the project)
publish         (node publish)
```

## Installation

```sh
curl -o ~/.config/fish/functions/yarr.fish --create-dirs https://raw.githubusercontent.com/simonrelet/yarr-fish-function/master/functions/yarr.fish
curl -o ~/.config/fish/completions/yarr.fish --create-dirs https://raw.githubusercontent.com/simonrelet/yarr-fish-function/master/completions/yarr.fish
```

**With [Fisherman](https://github.com/fisherman/fisherman)**

```sh
fisher install simonrelet/yarr-fish-function
```

## Usage

```
yarr script-name
```

## License

MIT.
