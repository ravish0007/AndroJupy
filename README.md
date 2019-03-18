 # AndroJupy
Hackish way to run jupyter notebook server in android platform


* Terminal-Emulator <br>
-->  termux

* Install termux from playstore<br>
[https://play.google.com/store/apps/details?id=com.termux](https://play.google.com/store/apps/details?id=com.termux)


<br>

* F-Droid (Alternative) <br>
[https://f-droid.org/repository/browse/?fdid=com.termux](https://f-droid.org/repository/browse/?fdid=com.termux)

<br>

* To play with explore down below <br>
[https://termux.com](https://termux.com) <br>
[https://wiki.termux.com/wiki/Main_Page](https://wiki.termux.com/wiki/Main_Page)

<br>
<span> <b>Step 1 :</b> Open the termux app for initial setup. </span>
<br>
<span> <b>Step 2 :</b> Go to settings/App and Enable storage permission to the app  </span>
<br>
<span> <b>Step 3 :</b> Open termux & execute <b>'termux-setup-storage'</b> (without quotes and this allows storage access Internal sdcard)  
<br> 
<br>
<b>Step 4 : Execute the following </b> <br>
<br> 
  
* <b> pkg update </b><br>
* <b> pkg install proot </b> ('creates Unix/Linux Tree, fake root for building apps')  <br>
* <b> termux-chroot </b> <br>
* <b> apt install git clang </b><br>
* <b> apt install pkg-config  </b><br>
* <b> apt install python python3-dev </b>('python 3.x & Python.h') <br>
* <b> apt install libclang libclang-dev </b><br>
* <b> apt install libzmq libzmq-dev </b><br>
* <b> apt install ipython </b> ('Interactive python') <br>
* <b> pip install jupyter </b> <br>
<br>
<b>Step 5 : Execute <i>jupyter-notebook</i></b> <br>

- By now you should be able to see the jupyter notebook server running with a generated URL.<br>
Long pressing on the console should give you two selecting cursors for selecting the URL and paste it into any browser.<br>
You will be in jupyter home directory.

<b> Tips:</b>
* Simultaneously pressring <b><i>Up Volume</i></b> button and <b><u>q</u></b>  on your keyboard should add additional keys panel while you're in <b>Termux</b>.
* <b> apt install scipy </b> [SciPy.org](https://scipy.org)
* <b> apt install numpy </b> [NumPy.org](http://www.numpy.org) 
* <i> These are compiled binary modules, <u>Installation of numpy in this manner is not recommended if you're installing Matploitlib</u></i>
* <b>Install qpython</b>  [Qpython.com](https://www.qpython.com)
* [Google_Play](https://play.google.com/store/apps/details?id=org.qpython.qpy)
* [AppLink_Github](https://github.com/qpython-android/qpython/releases/download/v2.4.0/Qpython_2018-09-29_google.apk)
* Open <b>Qpython</b> for intial setup, and also switch to Python3 in the app ('It will download additional scripts') 
* <b>Install Qpython_Notebook</b>  [Qpython @GitHub](https://github.com/qpython-android/notebook)
* [Google_Play](https://play.google.com/store/apps/details?id=org.qpython.notebook)
* [AppLink_Github](https://github.com/qpython-android/notebook/releases)
* Open <b> QpythonNotebook </b> for initial setup, it switches to <b> Qpython</b> app where you need to enable notebook service and to download few resource.<br>
* Close <b>Qpython</b> and <b> QpythonNotebook </b>, Open <b>Termux</b>.<br>
* Change directory to '<i>/sdcard/qpython/notebook</i>' by executing <b> cd /sdcard/qpython/notebook</b>, try <b> exit </b> because of <b>termux-chroot</b>, you need to play with this if <b>QpythonNotebook</b> doesnot work, just create necessary  folders by looking at http requests in <b>Termux</b>.
* Execute <b>jupyter notebook --NotebookApp.token=qpythonotebook --port 13000 </b>
* Open <b> QpythonNotebook</b>, play around with shortcut buttons, Install [hackers_keyboard](https://play.google.com/store/apps/details?id=org.pocketworkstation.pckeyboard) which gives good feeling in <i> landscape </i> mode.

<br>
<br>

* <b> Installing section of <i>   [Matplotlib](https://matplotlib.org/) </i> </b>
  <br>
  
  * <b>Step 1 :</b> Install Dependencies,<b> <i> apt install libpng libpng-dev freetype freetype-dev</i></b><br>
  * <b>Step 2 :</b> Installing qhull library,<br><br>
  <b>  git clone https://github.com/qhull/qhull.git ; \ <br> 
   cd qhull ;  \ <br>
   make ;  \ <br> 
   export  LD_LIBRARY_PATH=$PWD/lib:$LD_LIBRARY_PATH  <br>
   cd ..  </b><br><br> 

  * <b>Step 3 :</b> Remove Numpy,<b> <i> apt remove numpy </i></b>, If its being installed from Termux repository. <br>
  * <b>Step 4 :</b>  Install  Numpy from Pypi,<b> <i> pip install numpy </i></b>, This is because compiled one wont be detected while setting up matplotlib <br>
  * <b>Step 5 :</b> Install matplotlib from pypi,<b> <i> pip install matplotlib </i></b> <br>
<br>  
<b>Please be patient during the process.</b>
<br>
<br>

<img src="https://github.com/ravish0007/AndroJupy/blob/master/Image_1.png" width="360" height="640">

<img src="https://github.com/ravish0007/AndroJupy/blob/master/Image_2.png" width="360" height="640">

<br>
<br>
Thanks to @Qpython @Ipython communities and @ThePSF
Share your experience and for further more write to me @ <email>4al16cs077@aiet.org.in</email>

  
  
