# docker-pelican

docker composition for static [Pelican](https://github.com/getpelican/pelican-plugins) based web sites with webhook auto builder

# Install

```
git clone --recursive https://github.com/yomguy/docker-pelican.git`
```

This will also checkout all pelican plugins. To get all pelican-themes:

```
cd lib/pelican-themes
git submodule update
```

# Configure

The config file is `app/pelicanconf.py`

# Get text sources

You will need a separate repository for your text sources. Clone it in the var/in directory, for example:

```
cd var
git clone https://github.com/yomguy/musichacking2017.git
```

# Start

```
docker-compose up
```

# Trigger

The app can automatically be triggered by a webhook as explained [here](https://github.com/yomguy/pelicangit)

# Enjoy!

with love <3

# License

docker-pelican is free software: you can redistribute it and/or modify
it under the terms of the GNU Affero General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

mezzanine-organization is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU Affero General Public License for more details.

Read the LICENSE.txt file for more details.
