# dot-log-viewer

No install, just debug it in 1 minute.   
A simple .log file viewer in php
### Demo
[https://craftpip.github.io/dot-log-viewer](https://craftpip.github.io/dot-log-viewer)

### Features
- Easy setup, single file, just copy the dotlogviewer.php file in whatever directory.
- View files from multiple log directories.
- Scroll through the logs in reverse order (newest first).
- Easy navigation to next and prev logs, no matter how long that string is.

### Installation
- Download the dotlogviewer.php file
- Edit the file to set the `$paths` to your log directories
```php
class DotLogViewer {
    private $paths = [
        '../my-project/api/storage/logs', // latest file from this directory will be viewed by default
        '../bananas/app/logs',
    ];
... 
```
- open dotlogviewer.php in your browser with apache
- or create a local server `php -S localhost:8080` and open [http://localhost:8080/dotlogviewer.php](http://localhost:8080/dotlogviewer.php)


###  License

Copyright (C) 2023 Boniface Pereira   
Licensed under the MIT license.
