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

PHP Coding Lessons 101
---

**PHP Tags / Printing / Comments**

Tricks
1. Instead of using echo or print, you can use <?= 'Your Text' ?>
2. 'echo' can be used to make a list of things; however, 'print' cannot do so.
3. '<br>' is used to separate the new line.
4. don't forget to put ; at the end of each line.
   
```
<?php
// This is a single-line comment
echo 'This is an echo statement';
echo '<br>';
print 'This is a print statement';
print '<br>';
// We can echo more than one string at a time by separating them with a comma
echo 'This is line 1', 'This is line 2';
echo '<br>';

/*
    This is a multi-line comment
    This is line 2
    This is line 3
  */
?>
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="https://cdn.tailwindcss.com"></script>
    <title><?php echo 'Learn PHP From Scratch'; ?></title>
</head>

<body class="bg-gray-100">
    <header class="bg-blue-500 text-white p-4">
        <div class="container mx-auto">
            <h1 class="text-3xl font-semibold"><?= 'Learn PHP From Scratch' ?></h1>
        </div>
    </header>
    <div class="container mx-auto p-4 mt-4">
        <div class="bg-white rounded-lg shadow-md p-6">
            <h2 class="text-2xl font-semibold mb-4"><?= 'Welcome to the course' ?></h2>
            <?= '<p>In this course, you will learn the fundamentals of the PHP language</p>' ?>
        </div>
    </div>
</body>

</html>
```

**Variables**
Containers that hold data that you can later use to access that data or value. Variables can hold different types of data (strings, integers, boolean, etc.).

$name = 'Brad'
Rules 
  1. Prefixed with a dollar sign ($)
  2. Start with a letter or an underscore / not with a number 
  3. Can only contain letters, numbers, and underscores.
  4. Case sensitive

Variables Naming Convention
  1) Underscore: $server_name => 
  2) Camel Case: $ => Custom variable
  3) Pascal Case: $ServerName => classes
  4) Lowercase: $servername => database parameters variable

```
<?php
$title = 'PHP From Scratch';
$heading = 'Welcome to the course';
$body = 'In this course, you will learn the fundamentals of the PHP language';
?>

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="https://cdn.tailwindcss.com"></script>
    <title><?= $title ?></title>
</head>

<body class="bg-gray-100">
    <header class="bg-blue-500 text-white p-4">
        <div class="container mx-auto">
            <h1 class="text-3xl font-semibold"><?= $title ?></h1>
        </div>
    </header>
    <div class="container mx-auto p-4 mt-4">
        <div class="bg-white rounded-lg shadow-md p-6">
            <h2 class="text-2xl font-semibold mb-4"><?= $heading ?></h2>
            <p><?= $body ?></p>
        </div>
    </div>
</body>

</html>
```

