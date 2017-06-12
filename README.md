##### Sublime Text 3安装[packagecontrol](https://packagecontrol.io/installation)

<p><kbd>ctrl<em>+</em>`</kbd></p>

```
import urllib.request,os,hashlib; h = 'df21e130d211cfc94d9b0905775a7c0f' + '1e3d39e33b79698005270310898eea76'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
```

Click the `Preferences > Browse Packages…`menu
Browse up a folder and then into the `Installed Packages`/ folder
Download [Package Control.sublime-package](https://packagecontrol.io/Package%20Control.sublime-package) and copy it into the Installed Packages/ directory
Restart Sublime Text
