# PHP From Scratch
Any progress toward learning PHP as a secondary backend language by executing via server-side language.  

Server-side code is executed on the server. It is not accessible from the browser. Only the output from the code is accessible. Unlike, the client-side code e.g. JS is executed within the browser. All client-side code is visible to the user in the source code. 

- Security: Code cannot be seen by the client.
- More Efficient
- Database Access
- File System Access: writable and readible
- Authentication: log-in & register functionality
- Sessions

** Laragon is used to solve the flexibility weakness => install the full version of Laragon 

  [Download here: Laragon](https://laragon.org/)

To enable the local hosting, 
  1. Click "Start All"
  2. Click "Web" to display your localhost and view it
  3. Database can integrate MySQL and other database platforms
  4. Terminal => type command 'ls' to check the lists of file of your core server e.g. www

In the www. folder, create a folder and rename to anything as you wish and create index.php file. Now, you can edit 'index.php' file and your localhost will display it if formatted correctly. 

We can also embed HTML codes into PHP files.

In order to publish your localhost/folder-name or folder-name.test (make sure to use the right suffix the program or you set it up; .test is a default suffix) 

Before setting up localhost:8000, you should set up pathway to the executable php. In other words, if you use VSCode, go to "Preference" > "Settings" > search "PHP" > find "executable path.json" > look it up "bin" folder > copy file path and add "\\php.exe" > restart your VSCode to have the effects felt 

Basically, to set up your localhost:8000, type `php -S localhost:8000`.
