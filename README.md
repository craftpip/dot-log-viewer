# dot-log-viewer

![DotLogViewer](logo.png | width=100)

No install, just debug it in 1 minute.   
A simple .log file viewer in php

### Features
- Easy setup, single file, just copy the dotlogviewer.php file in whatever directory.
- View files from multiple log directories.
- Scroll through the logs in reverse order (newest first).
- Easy navigation to next and prev logs, no matter how long that string is.

### Installation
- Copy the dotlogviewer.php file into your directory
- Edit the file and set the $paths to your directory
```php
class LogsViewer {
    private $paths = [
        '../myproject/api/storage/logs', // latest file from this directory will be viewed by default
        '../anotherproject/laravel/storage/logs',
    ];
```
- open dotlogviewer.php in your browser with apache
- or create a local server `php -S localhost:8080` and open [http://localhost:8080/dotlogviewer.php](http://localhost:8080/dotlogviewer.php)
