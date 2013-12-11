Memorandum of Preferences.sublime-settings for me.

Move the original Preferences.sublime-settings file
$ mv ~/Library/Application\ Support/Sublime\ Text\ 3/Packages/User/Preferences.sublime-settings ~/git/st3/

Put a symbolic link
$ ln -s ~/git/st3/Preferences.sublime-settings ~/Library/Application\ Support/Sublime\ Text\ 3/Packages/User/Preferences.sublime-settings

======================================================
*Install PackageControl*
1. Show Console: control + `
2. Paste: import urllib.request,os; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); open(os.path.join(ipp, pf), 'wb').write(urllib.request.urlopen( 'http://sublime.wbond.net/' + pf.replace(' ','%20')).read())
3. Enter

======================================================
