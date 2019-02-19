  **x-quickapk home**

x-quickapk is a **GNU/linux** tool for building APK packages from [RFO-BASIC!](http://rfo-basic.com/) sources.

x-quickapk  was greatly inspired by [Quick APK](http://mougino.free.fr/quickapk.html) for Windows by Nicolas Mougin.

**x-quickapk is released under** **GNU/GPL license****.**

Read NOTICE inside source package for included tools licenses.

x-quickapk needs: 

\* Gambas 3
\* Java JDK 1.7 or OpenJDK-jdk 1.7 (jre is not sufficient)

x-quickapk was written using Gambas QT components. If you run x-quickapk under a GTK desktop environment, 
please run qtconfig and select GTK as theme. x-quickapk will look then as a GTK program.

To build an APK from your RFO-BASIC! program do:

mkdir foobar

cd foobar

mkdir source
mkdir data
mkdir databases

Copy all your basic files to "source" directory
Copy data files needed by your App to "data" directory
Copy databases (if any) to "databases" directory

At the moment, making data and databases folders is mandatory, 
even if your program does not need data files or databases.

**WARNING: x-quickapk uses openssl to encrypt your keystore.** **If openssl****is missing, keystore password is saved CLEARLY in $HOME/.config/gambas3/x-quickapk.conf**

From command line run:  ./x-quickapk

or you can click the binary icon.

Options for command line:

**-debug** Save all source files, builder-error.log, x-quickapk.project to $HOME/appname-debug_date_time

**-version** Print x-quickapk version  

**-nobt** Don't check versions on bintray.com

**-xfce** Useful if you run x-quickapk on XFCE  

**-help** Show options

Configure your App. GUI should be intuitive.

[![x-quickapk screenshot](http://rfo-basic.com/x-quickapk.png)](http://rfo-basic.com/x-apk-builder.png)

**Download source**: [xqa-20150515-mod-humpty-v3.zip](http://laughton.com/basic/programs/tools/x-quickapk/xqa-20150515-mod-humpty-v3.zip)
Source md5sum: f73ecfbfedbdc326e8690220e08ef2ca

To compile, do:

unzip xqa-20150515-mod-humpty-v3.zip

cd xqa-20150515/xqa

sh build.sh

Questions, comments, bug reports ---> [http://rfobasic.freeforums.org/questions-or-comments-about-basic-f4.html ](http://rfobasic.freeforums.org/questions-or-comments-about-basic-f4.html)

x-quickapk author: Stefano Palmeri
mod by humpty     