Java3DGameEngine
================

Java 3D game engine using lwjgl2.9.1 libraries for OpenGL portability and slick libraries for textures. This project is built and deployed using Gradle

Navigation
-----------
[Java3DGameEngine](#java3dgameengine) |
[Abstract](#abstract) |
[Screenshot](#screenshot) |
[Configuration](#configuration) |
[JAR and Natives Configuration](#JAR and Natives Configuration) |
[Folder Structure](#Folder Structure) |
[Running the program](#running the program) |
[License](#license) |


Abstract
-------
Java3DGameEngine is a fully functional game engine with a few items thrown in and movement enabled so that you can "fly" around a scene I have created. Variations on an old tutorial series by @BennyQBD

Screenshot
----------
![Picture](http://rabbitfighter.net/wp-content/uploads/2014/12/Java3DGameEngine.png)


Configuration
==============================
This program requires jars as well as natives for Windows, Linux, and OSX in the lwjgl vers 2.9.1 ZIP file. As per our Gradle build program, these files must be obtained and put into the correct folders in the project structure or you will be an unhappy camper, and the program will fail. So the following steps are necessary:

JAR and Natives Configuration
-----------------------------
<ol>
<li>Obtain the LWJGL (vers 2.9.1) zip file from: http://legacy.lwjgl.org/ and extract the files somewhere.</li>
<li>Obtain the Slick2D zip file from: http://slick.ninjacave.com/ and extract the files somewhere.</li>
<li>Create a folder in the main directory of the project called <code>libs/</code></li>
<li>Create a subfolder in the <code>libs/</code> folder called <code>jar/</code></li>
<li>Move the native folder from wherever you extracted the lwjgl.zip folder, and then move the whole folder into the <code>libs/</code> folder in the project.</li>
<li>Copy <code>lwjgl.jar, lwjgl_util.jar, jinput.jar</code> from the extracted files and move it into the <code>libs/jar/</code> folder in the project.</li>
<li>Copy <code>slick.jar</code> and <code>slick-util.jar</code> from the extracted files and move it into the libs/jar/</code> folder in the project.</li>
</ol>

Folder Structure
----------------
<pre>
.
├── build.gradle
├── libs
│   ├── jar
│   │   └── lwjgl.jar
|.. |.. └── lwjgl_util.jar
|.. |.. └── jinput.jar
|.. |.. └── slick.jartree
|.. |.. └── slick-util.jar
│   └── native
│       ├── freebsd
│       ├── linux
│       ├── macosx
│       ├── solaris
│       └── windows
├── LICENSE
├── README.md
├── res
│   ├── shaders
|.. |.. └── phongFragment.fs
|   │   └── phongVertex.vs
│   ├── textures
|.. |.. └── rock1.png
|.. |.. └── moss.png
├── src
│   └── main
│       └── java

13 directories, 14 files

</pre>

This should be your folder structure before running any commands.

Running the Program
-------------------
<ol>
<li>If gradle is not installed, install it. Then from the project directory, run <code>gradle build</code>.</li>
<li>Run the program by typing <code>gradle runJar</code></li>
</ol>

The program should run now. Yay!

Liscence
---------
Apache Licence 2.0







