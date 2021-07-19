# ps-startwebdev
We, developers, find it annoying or a teeny bit bothersome to set up our working directory for the same type of projects that we work on every single day or maybe even every other hour. I, as a web developer kinda found the solution to just spend a little less time in making the directory 😅.
For web developers, the most common directory setup will be 

1.  assets 🖼️   {  for dumping all pictures, icons etc }
2. css 🖌️        { where we dump all CSS files }
3. js ⚙️           { folder for associated JavaScript }
4. pages 📃    {for additional pages to be added to the website }
5. index.html  { the main page ! }

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1626611580023/iAF0hMVBoe.png)

There may be other directory setups too. I would love to know if there are any others. So once I found myself making folders manually every time I initiate projects...

for example

I used commands like ``` mkdir ``` or ``` touch [filename.extension]``` for every directory or file I make and admit it we do hate relying on the mouse at some point or the other. I wanted to automate / semi-automate the whole process. So at first, I figured out all the exact commands I used for setting up the project directory... and they were something similar to this in the command shell / PowerShell 
```
> mkdir assets 
> mkdir css ;cd css;touch style.scss
> mkdir js;cd js;touch app.js
> touch index.html

```
### 1. Eureka! 

And I had heard of something called .bat file..which is supposed to run a bunch of windows commands when we run it and Eureka ✨! 
All I had to do was figure out how to turn the above code into a .bat file ...And it turns out that I had to simply write what I want the bat file to do in the bat file in the command language. After some improvements and additions, my .bat file looked like this 
```
mkdir css; 
mkdir js; 
mkdir assets;
mkdir pages;
echo /* css/style.css */ > css/style.css
echo // js/script.js > js/script.js  
touch index.html

```
### 2. Converting .bat file into .exe file 
There were many converters online and there was this one converter that just did the thing I wanted it to do ~
[.bat to .exe converter](https://www.majorgeeks.com/files/details/bat_to_exe_converter.html)  from  [Major Geeks](https://www.majorgeeks.com/) and i simultaneously found a [ Software Walk Through](https://appuals.com/batch-to-exe/) 
 guide. The first part of the guide used something called IExpress which was manually converting that batch file into a package and then to a .exe file...but the second part had a more automated approach...where you just write the batch file and it will give you the .exe file when you press convert..Fairly straightforward! 

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1626614588452/FmXQQ-6Rc.png)

### 3. > start webdev
To successfully implement... `start webdev`...
once I had the .exe file ready with the name webdev, I had to save it in  `C:\Windows`.Why? because I had recently learned that any executable file in `C:\Windows` directory is directly accessible and can be opened by the command prompt or PowerShell just by writing the command `start program_name`, hence the path. After all these steps you are good to go 🏃🏻‍♂️! 

Here is the final execution of the whole process 😁

![startwebdev.gif](https://cdn.hashnode.com/res/hashnode/image/upload/v1626616382322/3UX3jau8_.gif)

You can customize the .bat file or you can create a whole new one and repeat the steps  for other project setups.
I invite you to create **safe** .bat files for other project setups too..










