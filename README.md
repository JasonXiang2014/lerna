# lerna
lerna parctice

https://github.com/lerna/lerna

## lerna 基本流程
### 全局安装
npm install lerna -g
### 创建目录、初始化
mkdir lerna & cd lerna
lerna init
### 添加package
mkdir lerna-module-1 & cd lerna-module-1 & npm init -y 
mkdir lerna-module-2 & cd lerna-module-2 & npm init -y
lerna add lerna-module-1 --scope lerna-module-2
### clean
lerna clean
### bootstrap
lerna bootstrap
### ls
lerna ls
### run
lerna run --scope lerna-module-1 test
### exec
lerna exec --scope lerna-module-1 -- ls
lerna exec --scope lerna-module-1 -- rm -rf ./node_modules






