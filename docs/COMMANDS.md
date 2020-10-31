# Commands

Below is  a list of built-in gulp tasks that can be used with StartQuick. StartQuick uses gulp to help automate repetitive tasks and take care of the boring work. Here are the built-in commands that activate certain functions.

### Synopsis:
  ```gulp command```

### Commands:

```help```	- Help; display a summary of  these  commands. If you forget all other commands, remember this one.


```start```	- This command creates and auto launches a  live development server in your default web browser. It will also compile your SASS files and automatically refresh the page when you make and save any changes in your project's files.

```compile```	- This command compiles and builds all of your source code into a folder called 'prod/' that is in the root folder of this project for deploying into production.

```clean```	- Delete the 'dev/' folder that contains your compiled project files, for use with the live server.

```fresh```	- Delete the 'dev/' and 'prod/' folders that contain your compiled project files, for use with the live server and production build, respectively.

### Examples

```
gulp start
```
Will start the live server. This will also result in a ```dev/``` folder being automatically created and populated  inside of your project's root directory with the files needed for your site to display on the live server.

```
gulp compile
```
Will result in producing a ```prod/``` directory with all of your minified ```.css``` and ```.js``` files, along with your images and ```.html``` files.

```
gulp clean
```
Will delete the ```dev/``` directory that was automatically created when using the ```gulp start``` command.

```
gulp fresh
```
This command will delete the ```dev/``` and ```prod/``` directories respectively. Cleaning up the project's build folders and leaving behind the source code only.
