# File Type Library
This library provides a set of functions to handle file types and their associated MIME types.
It allows you to get the MIME type of a file based on its extension, and also to get the file extension from a given MIME type.

The library uses a predefined dictionary of MIME types and their corresponding file extensions.
These are defined in the Library/AppSrc/mimeext.txt file.

## Backend: Libmagic
This library uses the unix/linux backend called "libmagic".
* It is a library that provides a way to identify the type of data in a file by examining its contents.
* It is commonly used in Unix-like operating systems to determine the type of a file based on its content rather than its filename or extension.
* It is often used in conjunction with the `file` command, which uses libmagic to identify file types.
* It is a powerful tool for file type detection and is widely used in various applications and programming languages.
libmagic uses a database of magic numbers and patterns to identify file types. It is called magic.mgc and in this case is located in the Library/Programs directory as its loaded at runtime as opposed to the mimeext.txt file which is loaded at compile time.

The Windows build is provided by: https://github.com/julian-r/file-windows/releases