## 说明
本仓库用于备份 Mac 下 Sublime Text 3 的设置，包括插件、快捷键、自定义后缀名渲染格式等等

## 原理
备份 Sublime Text 3 所在目录下的 Installed Packages 和 Packages 文件夹

```sh
cd ~/Library/Application\ Support/Sublime\ Text\ 3
# 接下来按 Git 的操作 Push 即可
```

## 恢复

```sh
cd ~/Library/Application\ Support/Sublime\ Text\ 3
rm -rf Installed\ Packages
rm -rf Packages
git remote add origin https://github.com/Norcy/Sublime_Backup.git
git pull origin master
```