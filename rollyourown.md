## How to write your own packet ##

Because the packets used by Robotics and Beyond will be converted into web pages
using an automated process, the files in a packet must follow certain
conventions, listed here.

## File Structure of a packet ##

Every packet must have at least 4 files, with these names and 
corresponding contents:

| File Name   | Contents                                              |
|:------------|:------------------------------------------------------|
| `index.md`  | a write-up giving the general purpose of that packet. |
| `bom.md`    | a bill of materials                                   |
| `demo.md`   | a page with demos, or links to demos                  |
| `todo.md`   | ideas for modifications                               |

Additionally, a packet may include any of these files, again with standardized
names and corresponding contents:

| File Name     | Contents                                                                    |
|:--------------|:----------------------------------------------------------------------------|
| `circuit.md`  | a circuit, preferrably developed with [Fritzing](http://fritzing.org/home/) |
| `code.md`     | associated code                                                             | 
| `license.md`  | a licence for use                                                           |
| `glossary.md` | definitions of special terms                                                |    
| `faq.md`      | a list of FAQ's for this project                                            |
| `refs.md`     | a list of pointers to other relevant material                               |

A packet can include other text files, with arbitrary names, as long as they
are in the Pandoc Markup language.  A packet can also include any multimedia files that
your text files link to.

## Directory structure of the packet ##

The directory tree of the files is simple:

    / (top level)
      |-- index.md
      |-- bom.md
      |-- ...  (other required files or files with standardized names)
      / images
        | -- image1.png
        | -- image2.jpeg
        | -- avideo.mpg

## How to contribute an entire packet to Robotics and Beyond ##

Once your packet contains at least the required files, you can
request that your repo be included in the RoboticsAndBeyond account, just
send an email to:  ...

