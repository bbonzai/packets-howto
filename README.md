## Overview of the R&B Teaching Packets ##

In summer 2016, Robotics and Beyond began using "packets" of teaching materials to
support classes in the summer camp.  The packets serve to help:

* students to view lesson content online, any time, at their own speed.

* parents to know what's being taught, and to join in learning or teaching;

* teachers to prepare new class materials.

The first set of packets applied only to the introductory class on Microcontrollers.
Another set, focussing on the Raspberry Pi class, is in its beginning stages.

A great deal of help and criticism is needed to improve and expand the packets;
this web site is designed to show potential contribtors how to help. 

## What's in a "packet"? ##

A packet consists of 

* a number of plain text files and
* any supporting graphics.

The text files and the supporting graphics files will be presented on a web site
administered by Robotics and Beyond.  A packet can *reference* but not include
multimedia files.  More details on that restriction are given [here]().

The process of converting the files into a web site is automated.  This imposes
a number of requirements on the input files:

1.  It is assumed that the text files are plain text, marked up using 
[Pandoc Markdown](http://pandoc.org/MANUAL.html#pandocs-markdown).

2.  Certain files must have a standardized name (see below).

3.  Graphics files can be in any format that can be rendered by browsers (e.g., `JPEG`,
`PNG`,`ICO`, etc.). 

## How you can contribute ##

You'll need to begin by setting up your own account at 
[GitHub](https://github.com).  

Then you can either:

* Modify an existing file in one of the existing repos in the 
`RoboticsAndBeyond` account.  This process is called "forking" a project.  
To get started with a fork, follow [these guidelines](forking.html).

OR

* Write your own packet from scratch, and store it in your own account on 
`github` until you want it to be incorporated into the RoboticsAndBeyond account.  
To get started writing your own packet, please follow guidelines 
[here](rollyourown.html).  

If you want to make extensive changes to some packet, or if you want 
to create your own packet, then you will need to 
install `git` on your computer; `git` is open source software and 
can be downloaded from [git-scm.com](https://git-scm.com).
However, since the packets are simply a collection of plain text and image files, you
can, in principle, do all your work on line, and will not need to 
install `git`. 

In any case, the packets you will be modifying are stored in the account owned
by `RoboticsAndBeyond` on `github.com`.  Currently, this account contains
two repositories (aka "repos"):

* [microcontrollers.intro](https://github.com/RoboticsAndBeyond/microcontrollers.intro)
* [raspberrypi.intro](https://github.com/RoboticsAndBeyond/raspberrypi.intro)

You can modify any packet in either repo.

## What happens to my files? ##

Packets stored in the `RoboticsAndBeyond` account at `github.com` will be 
automatically retrieved and converted to web pages that will be presented on 
the Robotics and Beyond web site (TBD).

`Github.com` automatically renders any text file which is formatted using Markdown
into an HTML page viewable on your browser.  However, `github` uses a 
different dialect of Markdown (so-called "Github Flavored Markdown, or GFM) than
is used for the packets, there will be slight differences between the way the packets
will eventually be presented on the Robotics And Beyond web site and the way they
appear to be rendered at the `github.com` web site.

If you want to see *exactly* how your pages will be rendered on the
Robotics and Beyond web site before you upload them to `github.com`, 
then you'll need to install some tools: 

* [Hakyll](https://jaspervdj.be/hakyll/), a program written in the functional
programming language (Haskell)[];
 
* the Haskell tool chain, including the GHC compiler and associated libraries; and  

* [sigkill.hs](http://sigkill.dk/programs/sigkill.html), which is a menu-generator
for Hakyll.



