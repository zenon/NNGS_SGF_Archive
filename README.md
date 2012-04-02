No Name Go Server - the Game Records
=======================

The No Name Go Server (NNGS, nngs.cosmic.org), was a real-time game server to play the Game of Go by connecting over telnet using a protocol that was a copy of that of IGS (Internet Go Server).

NNGS existed until around may 2005.

The game archive 
----------------
The game records are still available from several sources. It contains 435.495 sgf-files in 130 folders (each for one month from 07/1995 until 05/2005).

The Licence
-----------
The first game record contains the following CoPyright-Tag:

  This game falls under the protection of GNU copyleft.
  Permission to reproduce this game is given, provided proper credit is given.
  There is no warrantee, implied or explicit.
  Use of this game is an understanding and agreement of this notice.

The last game record contains the following CoPyright-Tag:

  This game was played on the No Name Go Server
  Permission to reproduce this game is given.

I'll have a look whether there are more of them.

Technicalities
--------------
Be aware, I repeat: 435.495 SGF files. In 130 folders (one per month). 728 MB. Thats many many of small files.

I hoped git will pack the repository to less than 300 MB (so it fits into my github space). 
"git add ." took 3 hours. (Well, there was an virus scanner interfering, I believe.) The .git directory had 397 MB (and took 1.71 GB of NTFS). So I deleted it again, and instead added the SGF files in one 7zip packed archive.

So, currently I believe it to be unwise to put almost half a million files into one git repo. (If you can tell othewise, I'm happy to hear so.)

If you unpack this 7z-file into NTFS (this Redmondian file system), it will eat over 1.5 GB.

Todo
-----
The files don't completely fulfil the SGF standard. (http://www.red-bean.com/sgf/) A task for this project is to make them do. (They contain some dashes at the end, and sometimes closing brackets in comment elements.)

The games are of, well, varying quality, but this is the biggest collection of go games publicly available, so it should be easily available. That means 1. on github, and 2. syntactically correct, so not everybody has to build a custome parser.

