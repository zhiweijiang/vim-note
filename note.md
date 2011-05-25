# _My Note

## bash

>``cd fir-<tab>``  -> cd first	(Quick completion)

###path
>pwd -> printf rel path

>which command -> locate a command 

>abs path

>rel path

###mkdir

>``mkdir -p mydir1/mydir2``  -> will also create all directories leading up to the given directory that do not exist already. If the given directory already exists, ignore the error.
>``mkfifo -> assembly a FIFO file

###mv and cp

>``mv aa bb``   -> rename or move

>``cp aa bb``   -> copy

>``cp -a -> copy a Directory file

###rm
``rm -rf *.c`` -> delete *.c 

### kill
    kill -l -> find all sign type
    ps -aux -> View the current all processes
    kill -9 processnum -> KILL this process
    $? -> the recently pid
###sudo

>sudo    -> SuperUser do

>sudo su -> root

###chmod

>umask                     -> Process mask
>ugo                       -> user, group, others

>a                         -> all

>rwx                       -> read(4), write(2), execute(1)

>``chmod ug+rw mydir``     -> drw-rw----

>``chmod 664 myfile``      -> -rw-rw-r--

>``chmod +x [filename]``   -> Enable Run

>``sudo mv tool.sh /bin``  -> To install it and Enable it Run Everywhere

>Try to install the MarkDown.

###Mentioned

*  GUI       -> Command Line
*  ls        -> list
*  cd        -> Change Directory (No Folder)
*  cd       --> soon back
*  rm -r -f  -> delete the file
*  whoami
*  history
*  the music: _The Pretty Reckless_
*  [MarkDown.pl](http://daringfireball.net/projects/markdown/ "MarkDown")
*  ``gcc -I/path/to/header/``
*  ``ldd a.out``

***

##install

*  ``./configure`` -> make a Makefile 
*  ``make`` -> command Makefile
*  ``sudo make install`` -> Automatic configuration

### /bin

>``sudo mv tool.sh /bin``  -> To install it and Enable it Run Everywhere

###apt-get

>``apt-get update``

>``apt-get install git-core``   -> install the Git

>``wget 122.115.61.189/tmp/cc-note``   -> Download

###Mentioned

*  dpkg
*  ``dpkg -S /usr/include/stdlib.h``  -> -S --search

***

##vim

*  i               -> input
*  v               -> select
*  V               -> to select one line
*  CTRL+v          -> to select for square
*  u               -> UNDO
*  CTRL+r          -> ONDO
*  CTRL+c          -> Note for C program files
*  :h vim-modes    -> get help for modes
*  :w              -> write
*  ``:w hello.c``  -> write to hello.c
*  :q              -> quit
*  !               -> force
*  ,ss             -> setlocal spell
*  SHIFT+k         -> man
*  vimtutor        -> the vim tutor
*  :vnew/new file  -> CTRL+w+w to change window and :bd(buffer delete) to close active
*  :Tlist          -> we can use ",t" when use Peter's VimRC
*  :NERDTreeToggle -> we can usr ",n" when use Peter's VimRC
*  :bn             -> switch among buffers, (<tab> in Peter's VimRC)
*  :ls             -> vim's list
*  zf              -> Create floding.
*  zx              -> Open floding.
*  zc              -> Flod floding.
*  ``vim -t main`` -> should exist the ctags
*   :v  CTRL + x   -> Automatically indents
### split view

*  ``vim -On file1 file2``  -> Vertical Split
*  ``vim -on file1 file2``  -> Horizontal Split
*  Ctrl+w s                 -> Vertical Split
*  Ctrl+w v                 -> Horizontal Split
*  Ctrl+w c                 -> Close current window
*  Ctrl+w q                 -> Close current window and if it is the last window the Vim will exits.
*  Ctrl+w w                 -> Activate the next window.

### vim config

*  ``:set nu``          -> Show line number
*  ``:set autoindent``  -> Auto indent
*  ~/.vimrc             -> vim config
*  ``:h 'autoindent'``  -> for help

### ~.vim/snippets/

#### c.snippets(e.g.)

    # #include
    snippet inc
        #include <${1:stdio}.h>${2}

tandard

*  CTRL+N
*  CTRL+]
*  CTRL+O

###Auto completion

*  ``CTRL-N``    -> quick completion
*  ``CTRL-L-K``  -> set spell
*  ``CTRL-X-L``  -> quick completion line
*  ``CTRL-X-F``  -> quick completion the filename
*  ``CTRL-x-k``  -> check with the dictionary
*  Check ``:h i\_Ctrl-<tab>`` for help.

### find file

*  ``find .|grep filename``
*  ``locate stdlib.h``  -> and you can use ``sudo updatedb`` to update the datebase.

###Metioned

*  gedit
*  Search 'peter-vim' from github.com
*  [get Peters vimrc config](http://happypeter.github.com/GitBeijing/vim-conf-share.html) 
*  ~.vim/snippets/
*  Use stags for many files
*  get search from hen of Peters's github.
*  ``ps aux|grep -i firefox``   -> get help from manpage
*  ``kill -9 18576``
*  vimdiff file1 file2          -> Show diff of file1 and file2.
*  [vim.org](http://www.vim.org)

***

##Extract

*  ``unzip [filename]``   -> To extract the file[filename]
*  ``tar xzvf tig-0.17.tar.gz``   -> Extract .tar and .gz
*  ``tar czvf *.gz *.*  -> Decompress file
***

##diff

*  ``diff -u a.c b.c > c``   -> Show diff of 'a.c' and 'b.c' to file 'c'
*  ``patch file1 file2``   -> For file1 on the file2 patches.
*  vimdiff

***

##git

*  ``git init``   -> Create an empty git repository or reinitialize an existing one.
*  ``git add h.c`` -> Add file contents to the index
*  ``git commit -a -v -m "first version"``   -> Record changes to the repository. (-a: All the changes. -v: berbose. -m: Message)
*  ``git diff``   -> Show diff.
*  ``git reset --hard HEAD``   -> Reset current HEAD to the specified state.
*  ``git checkout <branchname> [-b <new branch name>]``
*  ``git branch [-d <branchname>]``   -> Show branch. -d for delete.
*  ``git branch [-m <old branchname> <new branchname>]``   -> Move/rename a branch and its reflo.

### ~/.gitconfig

    [user]
    name = Peter Wang
    email = happypeter1983@gmail.com
    [core]
    editor = vim
    [alias]
    ci = commit -a -v
    co = checkout
    st = status
    br = branch
    throw = reset --hard HEAD
    throwh = reset --hard HEAD^
    [color]
    ui = true

    [commit]
    template = ./.commit-template
    [push]
    default = current

### tig

>``d``   -> Show diff

###Mentioned

*  [tig](http://jonas.nitro.dk/tig/ "tig")
*  [Peter's book](http://happypeter.github.com/LGCB "Peter's book")
*  git clone https://github.com/happypeter/cc-note.git
*  [ProGit](http://progit.org "ProGit")
*  [Git book at progit web.](http://progit.org/book/zh/ "Git Book")
*  git pull   -> To update the git directory.
*  script -> Script usually is interpreted language. And run some functions of a specific program.
*  README
*  TODO
*  the book : _how to become a hacker_
*  git for review
*  wget 122.115.61.189/happycasts/happygit-zh/git_start.ogv
*  git branch
*  [linux set up git](http://help.github.com/linux-set-up-git/)

***

## .sh
    for file in `ls`
    do
        if [[ $file == *.md ]]; then
            echo $file
        fi
    done

***
#C

##file
       _Written text ending add '\n' by hand_
### feof
    while(!feof(fp))  -> C "language" feof () "function to return the last "read" operation of the content.   
### fopen
       wb+ ->  Open for binary file. outher function is same with w+
       w+  ->  Open for reading and writing.  The file is created  if  it  does not  exist, otherwise it is truncated.  
               The stream is positioned at the beginning of the file. 
  
       r+  ->  Open for reading and writing.  The stream is positioned  at  the beginning of the file.

       a+   ->  Open for reading and appending (writing at end  of  file).   The file is created if it does not exist. 
                The initial file position for reading is at the beginning of the file, but output is always  appended 
                to the end of the file. 
### Output terminal
    when char from buffer to output terminal
    one: met '/n'
    two: fflush(stdout);
    three: fflush full or Procedure ended
    (fflush just only empty output buffer)
### Regular expressions
    grep "/bFILE/b" *.h -R(cycle find) -> find FILE in *.h
### make
>      ls /dev/fb0
       ( if no   sudo chmod 777 /boot/grub/grub.cfg   add vga=0x318 in the grub.cfg ) 
       0x318 -> (width:1024 length: 768 bpp: 32)
>      ls /dev/input/mice

>       make -> make main
>       make run -> ./main
>       make clean

### Makefile

* #this is for chess game
    scr = main.c init_screen.c
    para = -o main -Wall
    main:$(scr)
            gcc $(scr) $(para)
    clean:
            rm -rf main
            rm -rf *.o
            rm -rf ~*
    run:
            ./mian
* #This is for easy function
    CFLAG = -Wall -c -fPIC
    LDFLAG =-shared
    #src = a.c b.c c.c
    src = $(wildcard *.c)
    #obj = a.o b.o c.o
    obj = $(patsubst %.c, %.o, $(src))
    CC = gcc    
    target = libstak.so
    all:$(obj)
            $(CC) $(obj) $(LDFLAG) -o $(target)
    %.o:%.c
            $(CC) $(CFLAG) -o $@ $<
    .PHONY:clean
    clean:
        rm -f *.o
        rm -f $(target)

### console interface
    Ctrl+l  ->  Clean the screen
    Alt+Ctrl+Shift+<F1>   ->     To the console interface  
    Alt+<F7>   ->  exit the consle interface
### fivechess
    error(fb0: Permission denied)
    do: sudo chmod 777 /dev/fb0

### gcc
    (four steps)
    one: gcc -E *.c -o *.i (define)
    two: gcc -S *i -o *.s  (compilation)
    three: as *.s -o *.o   (assembly)
    four: gcc *.o -o *     (link)
 
    gcc -o -> the other named
    gcc -I -> indicated *.h file
    gcc -L -> indicated lib*.so file
    gcc -g -> goto debug environment
    gcc -c -> generated .o file
### gdb
    prinf(p) -> the value variable
    next(n) ->  carray out a command
    step(s) ->  step to function
    start -> main function start
    break(b) num  -> set num line breakpoint
    continue(c)  -> go on perform next a command
    run -> run before debug or end
### ftp
    ftp 192.168.3.227
    anonymous
    get c-test.doc
    bye  

## library
    link name(*.so) -> use when compilation
    so name(main version number) -> use when run
    real name(version number complete) -> front two name point to the file
### static library
    gcc -c *.c
    ar rs(r->file  s->index)  lib*.so  *.o
    gcc main.c libc*.so  -o main
###  shared library
    gcc -fPIC( related position) -c *.c
    gcc -shared -o lib*.so *.o
    gcc -I /include -L /lib*.so
### ldd
    ldd a.out
    libfive.so =>not found
    the first way: cp lib*.so /lib/lib*.so
    the second way: export LD_LIBRARY_PATH=/home/xwp/c-note/fivechess/main
    the three way: vim  /etc/ld.so.conf
                   sudo ldconfig -v
##Unbuffered IO
    int open(const char *pathname, int flags,...) 
    int close(int fd)
    ssize_t write(int fd, const void *buf, size_t count)
    ssize_t read(int fd, void *buf, size_t count)]
    off_t lseek(int fd, off_t offset, int whence); ->(Device settings cannot be offset)
    whence : SEEK_CUR -> file the current location
             SEEK_SET -> file start 
             SEEK_END -> file end 
    int fcntl(int fd, int cmd, strcut flock *lock);
    " < " -> default 0 stdin write only  
    " 2<* " -> 2 redirection *
    " > " -> default 1 stdout read only
    " >> " -> additional way to write
    " <> " -> redirevtion read and write
    int ioctl(int d, int request, ...)
    void *mmap(void *addr, size_t len, int prot, int flag, int filedes, off_t
    off)
    od -> dump files in octal and other formats
    $ vi hello
    $ od -tx1 -tc hello
    00000000 68 65 6c 6c 6f 6a
              h  e  l   l   o  \n
    00000006
    int fstat(int fd, struct stat *buf)
### Framebuff
    void *memset(void *s, int c, size_t n)->(function fills the first n bytes of the 
    memory area pointed to bys with the constant byte c
### Pictures format
    dd if(input file)= *.bmp of(out file)=image bs=54 sk:p=1 -> Intercept a 
    part of *.bmp make image
### Many programming process
    (gdb) set follow-fork-mode child
    int dup2(int oldfd, int newfd) -> makes newfd be the copy of oldfd,
    closing newfd first if  necessary
    ps u -> 
    xwp      17151 29.0  0.0   1532   284 pts/1    R    18:20   0:24 ./a.out
    xwp      17152  0.0  0.0      0     0 pts/1    Z    18:20   0:00 [a.o]
    <defunct>
    sudo kill -9 17151 -> kill 17152 zombie processes
    kill(pid, SIGINT) -> send a SIGINT sign to pid process
#_TODO_
*  To learn bash from Peter's website.
*  _Program Lib HOWTO_
*  http://vim-showoff-peter.heroku.com
*  [Seven habits of effective text editing](http://www.google.com.hk/search?sourceid=chrome&ie=UTF-8&q=Seven+habits+of+effective+text+editing)
*  To learn Linux c from song's website.
   Linux C
   http://learn.akae.cn/media/index.html
