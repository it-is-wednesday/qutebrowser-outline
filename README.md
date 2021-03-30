# Qutebrowser https://outline.com integration

Hi! This is a short [Qutebrowser userscript](https://qutebrowser.org/doc/userscripts.html) to fetch
the currently viewed URL's outline.com version, which makes it more readable. The script doesn't
redirect you to outline.com, but rather uses their API to fetch a clean version of the article,
saves the HTML locally (with some style touchups) and opens it in Qutebrowser.

After placing it in `~/.local/share/qutebrowser/userscripts`, you can use it with the following
command in Qutebrowser:
```
:spawn --userscript outline
```

You can also define an alias like this:
```
:config-dict-add aliases outline "spawn --userscript outline"
```

Now you can use it by just calling:
```
:outline
```
