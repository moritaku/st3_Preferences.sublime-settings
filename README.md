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
*Installed Packages*

[HowToUse]

1. Open PackageControl: ⌘+⇧+p

2. Select InstallPackage

3. Select Package

[Packages]

*Gist

*MarkDownPreview

*Bracket Highlighter

*Japanize

*AndyPHP

*Flatland

*SFTP

*jQuery

*MacTerminal

======================================================
*Japanize*

1. PackageInstall "Japanize"

2. Copy: cp -a /User/(USERNAME)/Library/Application\ Support/Sublime\ Text\ 3/Packages/Japanize/*.jp /User/(USERNAME)/Library/Application\ Support/Sublime\ Text\ 3/Packages/Default

3. Replace: *.jp => *

4. Copy: cp -a /User/(USERNAME)/Library/Application\ Support/Sublime\ Text\ 3/Packages/Japanize/* /User/(USERNAME)/Library/Application\ Support/Sublime\ Text\ 3/Packages/User

Reference: https://github.com/kik0220/sublimetext_japanize

======================================================
*Use for Terminal(bash)*

1. $ vi ~/.bash_profile

2. Add: alias st="/Applications/Sublime\ Text.app/Contents/SharedSupport/bin/subl"

[HowToUse]

1. $ st FILENAME or DIRECTORYNAME

2. Open ST3 to FILENAME or DIRECTORYNAME