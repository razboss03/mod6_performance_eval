# CSE330
Razi Khan 498977 Razboss03

The server is actively running in the EC2 instance. These links should be active. If they are not please email k.razi@wustl.edu and I will look into it immediately. 

## Links to files:


[college photo](http://ec2-3-129-72-145.us-east-2.compute.amazonaws.com:3456/college.html)


[brookings](http://ec2-3-129-72-145.us-east-2.compute.amazonaws.com:3456/brookings.jpg)


[phpinfo.php](http://ec2-3-129-72-145.us-east-2.compute.amazonaws.com:3456/phpinfo.php)


[hello.txt](http://ec2-3-129-72-145.us-east-2.compute.amazonaws.com:3456/hello.txt)


## Why php is not served correctly:
node.js is not a web server. It is a static server. While we can have it serve files, it cannot go and compile other file types. We could use routes to have the file compile, but with the way we have it currently set up .php is not a known mimetype in the mime package and is thus compiled as plaintext and served to the end user.