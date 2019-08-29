```bash
theostangebye@theo-jetson:/usr/bin$ ls -l python
lrwxrwxrwx 1 root root 9 Apr 16  2018 python -> python2.7
theostangebye@theo-jetson:/usr/bin$ rm python
rm: cannot remove 'python': Permission denied
theostangebye@theo-jetson:/usr/bin$ sudo !!
sudo rm python
[sudo] password for theostangebye: 
theostangebye@theo-jetson:/usr/bin$ ln -s -T python3.6 python
ln: failed to create symbolic link 'python': Permission denied
theostangebye@theo-jetson:/usr/bin$ sudo !!
sudo ln -s -T python3.6 python
theostangebye@theo-jetson:/usr/bin$ ls -l python
lrwxrwxrwx 1 root root 9 Aug 29 12:41 python -> python3.6
theostangebye@theo-jetson:/usr/bin$ python
Python 3.6.8 (default, Jan 14 2019, 11:02:34) 
[GCC 8.0.1 20180414 (experimental) [trunk revision 259383]] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> 
```
