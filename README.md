# Dockerを使用したVueの開発環境
## How to move
Build the image of the container
```
% docker build -t app_name .
```
Start the container from the built image
```
% docker run -v `pwd`:/usr/src/app -p 9050:9050 --name app_name -it -d app_name
```
Go inside the container
```
% docker exec -it app sh
```
Project setup
```
% npm install
```
Create Vue project
```
% vue create .
```
