# wgetg
Open URL in graphical browser and return html source or save page as html file

**Demo:**

![Demo](wgetg.gif)

**Example: Open URL and return html source code**

By default the script opens the URL with firefox or chromium and returns the html source code of the web page.

```
$ ./wgetg https://example.com
<!doctype html>
<html>
<head>
    <title>Example Domain</title>

    <meta charset="utf-8" />
    <meta http-equiv="Content-type" content="text/html; charset=utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
...
```

**Example: Open URL with specific browser and save web page as HTML file with timestamp and page title in filename**

If a directory is set as `--outfile` ( `-o`), the filename will be "YYYY-MM-DDTHH-MM-SS.html" and the script returns this filename.

```
$ ./wgetg -t -b "google-chrome" -o "/home/foo" https://example.com
/home/foo/2022-05-15T12-55-01 Example Domain.html
```

