# FTP_Pull
This is a program written in Python3 that searches for files on a FTP site with a given extension and downloads them to a local folder. This program uses ftplib to access the server as well as logging to save a program log.

# Dependencies
This program relies on tqdm to work and show the progress of the downloading files. Run `pip3 install tqdm` using your computer's terminal to install it.

# How-To
To use the program properly, you'll need to provide it with a few variables. Go into the `FTP_Pull_RUN.py` file and change the following variables:

**username** The username that you use to login to your FTP site

**password** The password to login to your FTP site

**ftp_url** The URL that you use to access the FTP site. Don't include ftp://, just do ftp.website.com

**remote_directories** This list includes all of the folders that you want to pull from. If you want to search multiple directories for files, simply uncomment the first two lines and add in your file structure here. Just make sure to include '~/' in the beginning, that way it always returns to home and brances out from there.

**extensions** The program will only search for files with the correct extensions. It's currently configured to search for video files, but you can change that to whatever you want.

**overwrite** If set to True, the program will overwrite any local files that are not the same size as the remote files. If the program is disconnected for any reason, you can enable this to overwrite files that we're completely downloaded.

If you don't want to define these things, that's fine. You can run the program as-is and it will ask for the user to define the necessary variables.

# Help
If you need help, feel free to send me a message on GitHub. I'm still working out a few kinks in the program, so any constructive criticism is greatly appreciated.
