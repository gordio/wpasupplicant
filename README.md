# WPA Supplicant Python Lib

Python wpa_supplicant manager over D-Bus protocol.

_**WIP**: Work In Progress!_


### Dependencies

* wpa_supplicant
* python-dbus


### D-Bus Configuration

`/etc/dbus-1/system.d/org.freedesktop.ModemManager1.conf`:
```xml
<policy user="root">
    <allow own="org.freedesktop.ModemManager1"/>
</policy>
```

`/etc/dbus-1/system.d/wpa_supplicant.conf`:
```xml
<policy user="root">
    <allow own="fi.epitest.hostap.WPASupplicant"/>
    <allow own="fi.w1.wpa_supplicant1"/>
</policy>
```



## Contributing to a Project

• Prepare commit hook's:
```
pip install flake8 flake8-builtins flake8-docstrings
flake8 --install-hook git
git config --bool flake8.strict true
```

• Tests (TODO)



## License – MIT License

> Copyright (c) 2018 Oleh Hordiienko
>
> Permission is hereby granted, free of charge, to any person obtaining a copy
> of this software and associated documentation files (the "Software"), to deal
> in the Software without restriction, including without limitation the rights
> to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
> copies of the Software, and to permit persons to whom the Software is
> furnished to do so, subject to the following conditions:
>
> The above copyright notice and this permission notice shall be included in all
> copies or substantial portions of the Software.
> 
> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
> IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
> FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
> AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
> LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
> OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
> SOFTWARE.
