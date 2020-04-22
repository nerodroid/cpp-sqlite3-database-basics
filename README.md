# cpp-sqlite3-database-basics

This few files are to demo sqlite3 basics in C++

Steps for Setup


1.download mingw and install
http://mingw-w64.org/doku.php/download/mingw-builds

2.Update PATH ENV. VARIABLE with mingw bbin folder
default -C:\Program Files\mingw-w64\x86_64-8.1.0-posix-seh-rt_v6-rev0\mingw64\bin

3.Download Sqlite3 source code from https://www.sqlite.org/download.html
amalgamation for standalone library file so you can add it to your project

4.extract amalgamation files inside a folder and on CMD

gcc sqlite3.c -c
Will generate sqlite3.o (-c is compile only, generating object file)

5.And you have sqlite.o object file which will work with your c++ projects when you compile the object file with it

g++ main.cpp sqlite3.o -Ipath\to\sqlite3
(path is -isqlite3 if the .o file is in the same directory)

6.all the other files work in a simillar manner. 

External Source - https://www.devdungeon.com/content/compiling-sqlite3-c?fbclid=IwAR1-TO0r6UYHM-OWpqqZxVhiVKOk1eQeGrcN2mi5B1cwB2RnJx01PSuXPT8

