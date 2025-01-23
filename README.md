# Links-and-Images

Learning links and Images
Opening links in a new tab
The method shown above opens links in the same tab as the webpage containing them. This is the default behaviour of most browsers and it can be changed relatively easily. All we need is another attribute: the target attribute.

While href specifies the destination link, target specifies where the linked resource will be opened. If it is not present, then, by default, it will take on the _self value which opens the link in the current tab. 


<a href="https://www.theodinproject.com/about" target="_blank" rel="noopener noreferrer">About The Odin Project</a>


### noopener noreferrer
noopener:
Prevents the linked page from accessing or interacting with the original page.
Mitigates security risks like JavaScript manipulation of the original page.
noreferrer:
Hides the referrer information from the linked page.
Includes the behavior of noopener for additional security.
Why Use noopener noreferrer?

Security: Prevents phishing attacks like tabnabbing (e.g., opened link manipulates the original page to trick users).
Privacy: Prevents sharing referrer information with the linked page.
Best Practices:

Always pair target="_blank" with rel="noopener noreferrer" for enhanced security and privacy.
Modern browsers often implement noopener automatically for target="_blank", but explicitly adding it is recommended for robust coding practices.


###Absolute and relative links

Relative Links

Definition: Link paths relative to the current file or directory.
Example: about.html or ../images/logo.png
Advantages:
Shorter and easier to write.
Flexible when moving files within the same site structure.
Disadvantages:
Can break if the directory structure changes.

 Absolute Links

Definition: Full URL including protocol, domain, and file path.
Example: https://www.example.com/about.html
Advantages:
Always points to the same resource, regardless of location.
Ideal for linking to external websites.
Disadvantages:
Longer and more prone to errors.
Can break if the domain or URL structure changes.
Key Difference:

Relative links depend on the current file location.
Absolute links always include the complete URL.

### Images
We use img tag. with src attribute to link images. Can embed imgaes using both absolute and relative paths.


### Parent Directories 

A parent directory is the directory that contains the current directory. It is one level above the current folder in the file hierarchy.

Key Points:

Representation:

Represented as .. in file paths.
Example:
Current directory: /home/user/docs
Parent directory: /home/user
Usage:

Navigate up the directory structure.
Example:
../file.txt accesses file.txt in the parent directory of the current folder.
Common Applications:

Linking files or directories in relative paths.
Organizing and accessing resources in web development or file systems.
Benefits:

Simplifies file referencing in relative paths.
Avoids the need for absolute paths, making projects portable.
Note: Incorrect usage of parent directory references (..) can lead to broken links or navigation errors if the directory structure changes.
