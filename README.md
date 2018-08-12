# React JS enveriment configeration

## Using node and npm(package)
<br/>
run npm init:<br/>
Use  npm to generate project information: <br/>

![image](https://user-images.githubusercontent.com/15969187/43996974-390ac040-9d9d-11e8-8f86-531913ced24b.png)
<br/>
<br/>
instal react-dom and react modules<br/>
instal babel<br/>
instal webpack and webpack-dev-server<br/>
set path by create webpack.config<br/>
<br/>
# problem: 

![image](https://user-images.githubusercontent.com/15969187/43996997-0c0e1dc0-9d9e-11e8-8464-96a2b9162ae8.png)
<br/>
<br/>
Try to start the project and it went in to a problem:<br/>
Modul build failed:TyperError: fileSystem.statSync is not a function:<br/>
after resarch. this problem happen becuase when we install babel . we stall the newest version of babel which does not have fileSystem.statSync fucntion . there fore we need to degrade it to a lower version:<br/>
Use follow commend to instal verstion 7.1.1:<br/>
<br/>
npm install babel-loader@7.1.1 --save-dev<br/>
<br/>
now run the server
![image](https://user-images.githubusercontent.com/15969187/43997109-2a8bd79e-9da1-11e8-80ef-d730c626cfb2.png)
<br/>
<br/>
Test my web site.<br/>
the test website is display functionaly<br/>
The config is done.<br/>
