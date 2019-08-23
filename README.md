# [Traccar Web Interface](https://www.traccar.org)
[![Build Status](https://travis-ci.org/traccar/traccar-web.svg?branch=master)](https://travis-ci.org/traccar/traccar-web)

## Overview

Traccar is open source server for various GPS tracking devices. This repository contains web interface for the Traccar platform. For back-end checkout [main Traccar repository](https://github.com/tananaev/traccar).

Icons are generously provided by [Font Awesome](http://fontawesome.io/) and [Icons8](https://icons8.com/). We are also using [BrowserStack](https://www.browserstack.com/) to test compatibility with various platforms and browser versions.

## New version under construction

A new version is being developed https://github.com/traccar/traccar-web/tree/modern/modern

You can read about why write a new client here https://github.com/traccar/traccar-web/issues/592

## Deployment process

1. Install required binaries and sources, this part is executed once.
    ```bash
    wget https://www.dropbox.com/s/6xcajlcyn0hg68d/ext-6.2.0-gpl.zip && 
    wget http://cdn.sencha.com/cmd/6.7.0.37/no-jre/SenchaCmd-6.7.0.37-linux-amd64.sh.zip
    
    unzip SenchaCmd-6.7.0.37-linux-amd64.sh.zip
    ./SenchaCmd-6.7.0.37-linux-amd64.sh // follow instructions here
    unzip ext-6.2.0-gpl.zip
    ```

2. Run script
```bash
cd ./tools && ./minify.sh
```
You'll get app.min.js generated in `web` folder that's used by traccar in production.
No more steps needed, when traccar starts it'll spot this file and serve it statially 
by root path

## Team

- Anton Tananaev ([anton@traccar.org](mailto:anton@traccar.org))
- Andrey Kunitsyn ([andrey@traccar.org](mailto:andrey@traccar.org))

## License

    GNU General Public License, Version 3

    This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program. If not, see <http://www.gnu.org/licenses/>.
