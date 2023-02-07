# Mute Spotify adds
This project has been created and tested from a RHEL 8.7 OS using ALSA driver. Adapt to your needs.

## Setup

### Requisites
- Root access to your OS
- ansible core
- python3
- selenium libraries
`pip3 install selenium`
- [geckodriver](https://github.com/mozilla/geckodriver/releases) and/or [Chromedriver](https://chromedriver.chromium.org/downloads) under `/usr/bin/`


Run the `setup.yml` playbook that will install the requirements and the selenium script:
``` 
$ ansible-playbook playbooks/setup.yml -K
```

## Running the thing

The `setup.yml` playbook has placed in your `/usr/bin/` dir the `spotify-noads` script. Just run it in the background such:

```
$ which spotify-noads
/usr/bin/spotify-noads

$  spotify-noads &
```