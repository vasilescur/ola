# ola
CLI tool to generate quotes said by Professor Astrachan.

<img width="608" alt="screenshot of tool" src="https://user-images.githubusercontent.com/10100323/49537951-4d46c080-f898-11e8-959b-9f152f2a0ffb.png">

## Installation

### Requirements:

  - Must have Python 2 installed
  - `/usr/local/bin` must be on the path
  - `/usr/bin` must be on the path
  - Python 2's executable must be at `/usr/bin/python`

### Installing on MacOS or Linux:

To install, run the following commands:

```bash
git clone https://github.com/vasilescur/ola.git
cd ola
chmod +x ./install.sh
sudo ./install.sh
```

You may then delete the `ola` folder into which you cloned the repo.

### Installing on Windows

Clone or download the repository.

Rename the `ola` file to `ola.py`.


## Usage

### MacOS or Linux:

To use, simply run:

```bash
ola
```

If you want to use a different quotes source file, pass the path as an argument:

```bash
ola my_other_quotes.txt
```

Quote files are formatted as one quote per line.

You can also pipe output to other programs. For example:

```bash
ola | cowsay
```

The quotes file may be configured. It is stored at `/etc/ola/quotes.txt`.

### Windows

At the command line, run `python ola.py` from the repo's folder.

*Note*: Not tested, but this might break the ability to pass custom files as arguments (or might break the whole thing). If this is the case, maybe try find a fix by editing the `sys.argsv` section of the code.


## But why Python 2?

My Python 3 installation is a bit funky, so I decided to use Python 2 for more easy cross-platform support.

If you'd prefer to use Python 3, here's how:

  - In the main program (`ola` file), change `print message` to `print(message)`
  - Change the *shebang* line at the top of the file to point to your Python 3 executable

## Contributing

Pull requests are welcome. Please submit an issue if any bugs are encountered.

## Credit

Created by Radu Vasilescu.

Many of the quotes are sourced from here: [ola Quotes from CS 101](https://docs.google.com/document/d/1VGBr8D0jMmKrKgaDSdvMBAx9_EIu3jrYrjnbfnDS9Qk/edit?fbclid=IwAR1kZdFZo1wgNvPp3zBrpRTO_1EOTHPTHsf1AWVFc2KBZPU1WsG8Cga_vq4)

Others are added by me.

## License

MIT license. See `LICENSE` file.
