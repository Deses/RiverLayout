##### Original author David Ekholm (david@jalbum.net) http://www.datadosen.se/riverlayout/
## RiverLayout - a simple and flexible Java Layout Manager
Java is great but but designing user interfaces can be a headache, especially forms. Layout managers like FlowLayout and BorderLayout are easy to understand, but rather limited, and how often do you want components to wrap to the next row if a window is narrowed? (as is the case with FlowLayout). GridBagLayout is flexible all right, but apart from being overly complex and requiring one to write essays, one cannot easily modify the layout, say add a component in the middle, without having to adjust cell coordinates for other components.

I wanted a flexible layout manager that anyone can understand intuitively. Why not mimic how text is positioned in a text editor? In an editor words flow from left to right. They are normally separated with spaces, but if you want them aligned in columns you can use tab stops. You can insert line breaks where needed and even paragraph breaks to separate sections of text.

This is how RiverLayout works. Without further talking, look at the example below. It displays a simple form with a centered header and ok button. Two of the fields expand automatically to fill the available space and finally, the labels and fields are nicely aligned in two columns.

## Licensing
RiverLayout is released under the LGPL licence. You may therefore freely use it in both non-commerical and commercial applications and you don't need to open up your source code. Improvements made to RiverLayout should however be returned to the project for the benefit of everyone.

## Release history
1.1 (2005-05-25) -Bugfix: JScrollPanes were oversized (sized to their containing component) if the container containing the JScrollPane was resized.
1.0 (2005-04-24) Initial release

## Usage
To download this dependency just add this to the pom.xml

	<repositories>
		<repository>
			<id>RiverLayout-mvn-repo</id>
			<url>https://raw.github.com/Deses/RiverLayout/mvn-repo/</url>
		</repository>
	</repositories>
	<dependencies>
		<dependency>
			<groupId>se.datadosen.riverlayout</groupId>
			<artifactId>riverlayout</artifactId>
			<version>1.1</version>
		</dependency>
	</dependencies>

* * *

###### Published with permission of David Ekholm (david@jalbum.net).
