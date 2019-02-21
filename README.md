<a style="float:right;font-size:12px;" href="http://github.com/ionic-team/ionic-native/edit/master/src/@ionic-native/plugins/file/index.ts#L607">
  Improve this doc
</a>

# File

```
$ ionic cordova plugin add cordova-plugin-file
$ npm install --save @ionic-native/file
```

## [Usage Documentation](https://ionicframework.com/docs/native/file/)

Plugin Repo: [https://github.com/apache/cordova-plugin-file](https://github.com/apache/cordova-plugin-file)

This plugin implements a File API allowing read/write access to files residing on the device.

The File class implements static convenience functions to access files and directories.

Example:
```
import { File } from '@ionic-native/file';

constructor(private file: File) { }

...

this.file.checkDir(this.file.dataDirectory, 'mydir').then(_ => console.log('Directory exists')).catch(err => console.log('Directory doesn\'t exist'));

```

 This plugin is based on several specs, including : The HTML5 File API http: //www.w3.org/TR/FileAPI/
 The (now-defunct) Directories and System extensions Latest: http: //www.w3.org/TR/2012/WD-file-system-api-20120417/
 Although most of the plugin code was written when an earlier spec was current: http: //www.w3.org/TR/2011/WD-file-system-api-20110419/
 It also implements the FileWriter spec : http: //dev.w3.org/2009/dap/file-system/file-writer.html

## Supported platforms
- Android
- Browser
- iOS
- macOS
- Windows



