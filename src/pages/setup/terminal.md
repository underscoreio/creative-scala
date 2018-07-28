## Installing Terminal Software and a Text Editors

This section is our recommended setup for people new to programming, and describes how to setup Creative Scala with the terminal and a text editor.
We need to install:

- the JVM;
- Git;
- a text editor; and
- the template project for Creative Scala.


### OS X

Open the terminal. (Click the magnifying icon on the top righthand side of the toolbar. Type in "terminal".)

Install Java 8, if you have issues, see [this gist](https://gist.github.com/chriskaschner/541397736480c514cd561682ec34ce4f)

Type into the terminal

```bash
java
```

If this runs you already have Java installed.
Otherwise it will prompt you to install Java.

Install homebrew.
Paste into the terminal

```bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Install `git` using homebrew.
At the terminal, type

```bash
brew install git
```

Now install the text editor Atom.
Again type at the terminal

```bash
brew install Caskroom/cask/atom
```

Install Scala support inside Atom: Settings > Install > language-scala

Now we will use Git to get an SBT project that will work with Creative Scala.
Type

```bash
git clone https://github.com/underscoreio/creative-scala-template.git
```

<div class="callout callout-info">
#### Sharing Your Work {-}

There is an alternative setup that involves first forking the Creative Scala template project, and then cloning it to your computer.
This is the setup to choose if you want to share your work with other people; for example you might be taking Creative Scala with a remote instructor or you might just (quite rightfully) be proud of your work.

In this setup you first *fork* the Creative Scala template.
Then you make a clone of *your* fork.
This alternative setup is described in more detail in the section on GitHub later in this chapter.
</div>


Now change to the directory we just created and run SBT.

```bash
cd creative-scala-template
./sbt.sh
```

SBT should start.
Within SBT type `console`.
Finally type

```scala
Example.image.draw
```

and an image of three circles should appear!

If you've made it this far you've successfully installed all the software you need for work through Creative Scala.

The final step is to load Atom and use it to open `Example.scala`, which you can find in `src/main/scala`.


### Windows

Download and install Java.
Search for the "JDK" (Java development kit).
This will take you to Oracle's site.
Accept their license and download the JDK.
Run the installer you just downloaded.

Download and install Atom.
Go to `https://atom.io/` and download Atom for Windows.
Run the installer you've just downloaded.

Download and install Git.
Go to `https://git-scm.com/` and download Git for Windows.
Run the installer you've just downloaded.
At the very end it gives you the option to open Git.
Select that option.
A window will open up with a command prompt.
Type


```bash
git clone https://github.com/underscoreio/creative-scala-template.git
```

<div class="callout callout-info">
#### Sharing Your Work {-}

There is an alternative setup that involves first forking the Creative Scala template project, and then cloning it to your computer.
This is the setup to choose if you want to share your work with other people; for example you might be taking Creative Scala with a remote instructor or you might just (quite rightfully) be proud of your work.

In this setup you first *fork* the Creative Scala template.
Then you make a clone of *your* fork.
This alternative setup is described in more detail in the section on GitHub later in this chapter.
</div>

Open a normal command-prompt.
Click on the Windows icon on the bottom left of the screen.
In the search box enter "cmd" and run the program it finds.
In the window that is opened up type

```bash
cd creative-scala-template
```

which will change into the directory of the Creative Scala template project we just downloaded.
Type

```bash
sbt.bat
```

to start SBT.
Within SBT type `console`.
Finally type

```scala
Example.image.draw
```

and an image of three circles should appear!

If you've made it this far you've successfully installed all the software you need for work through Creative Scala.

The final step is to load Atom and use it to open `Example.scala`, which you can find in the directory `src\main\scala`.


### Linux

Follow the OS X instructions, using your distributions package manager to install software in place of Homebrew.
