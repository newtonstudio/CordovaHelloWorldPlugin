HelloWorldPlugin
============

This plugin allows you to study how to write a helloworld ios plugin, pass value into the plugin and return the value after process

Installation
------------

### For Cordova >= 3.0:

1. To add this plugin just type: `cordova plugin add https://github.com/newtonstudio/CordovaHelloWorldPlugin` or `phonegap local plugin add https://github.com/newtonstudio/CordovaHelloWorldPlugin`
2. To remove this plugin type: `cordova plugin remove com.iteatech.helloworldPlugin` or `phonegap local plugin remove com.iteatech.helloworldPlugin`


Usage
-------
<!doctype html>
<html lang="en" ng-app="app">
    <head>
       <title>helloWorld</title>
       <script src="cordova.js"></script>
    </head>
<body>
    <script>
        document.addEventListener("deviceready", function () {
                                  
           HelloWorldPlugin.echo(function(e){
                                 alert(e); //ios will return the value you pass into
                                 },function(){
                                 alert('fail');
                                 }, "anything to pass to ios here");
                                  
        },false);
    </script>
</body>
</html>
