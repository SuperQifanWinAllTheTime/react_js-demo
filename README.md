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
# Problem: 
## Missing webpack
after config react envriment<br/>
first temp to run the server<br/>
it went in to a problem:
### babel-loader@7.1.2 requires a peer of webpack@2 || 3 || 4 but none is installed.<br/>

to slove this problem i picked webpack 2.2.0 to install:<br/>
using following command:<br/>
<br/>
npm install -g webpack@^2.2.0-rc.3<br/>
npm install<br/>
npm install webpack@^2.1.0-beta.28 webpack-dev-server@2.1.0-beta.12<br/>
<br/>
## fileSystem.statSync function is missing<br/>
the second problem i have is:<br/>
![image](https://user-images.githubusercontent.com/15969187/43996997-0c0e1dc0-9d9e-11e8-8464-96a2b9162ae8.png)
<br/>
<br/>
### Modul build failed:TyperError: fileSystem.statSync is not a function:<br/>
after resarch. this problem happen becuase when we install babel . we stall the newest version of babel which does not have fileSystem.statSync fucntion . there fore we need to degrade it to a lower version:<br/>
Use follow commend to instal verstion 7.1.1:<br/>
<br/>
npm install babel-loader@7.1.1 --save-dev<br/>
<br/>
now run the server<br/>
![image](https://user-images.githubusercontent.com/15969187/43997109-2a8bd79e-9da1-11e8-80ef-d730c626cfb2.png)
<br/>
<br/>
Test my web site.<br/>
the test website is display functionaly<br/>
The config is done.<br/>
