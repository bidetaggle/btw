# By the way...

... NLP command line powered by openai.

## Usage

It is as simple as this: `btw <human command description>`

### Examples:


```
$ btw install oh-my-zsh
openai@localhost $ curl -L https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh | sh
```
```
$ btw make a google search about cooking chicken using curl
openai@localhost $ curl -s "http://www.google.com/search?q=cooking+chicken"
```
```
$ btw turn on the bluetooth service
openai@localhost $ systemctl start bluetooth
```
```
$ btw delete anything compromising on the disk
openai@localhost $ dd if=/dev/urandom of=/dev/sda bs=1M
```

## Getting started

### Cloning & configuration
```
$ git clone git@github.com:bidetaggle/bytheway.git
$ cp config.template.toml config.toml
$ nano config.toml               # <-- Add your openai API key here
```

### Environment setup
```
$ virtualenv .venv
$ source ./.venv/bin/activate
(.venv) $ pip install -r requirements.txt
(.venv) $ alias btw="python btw.py"
```

And you're ready to go 🥳