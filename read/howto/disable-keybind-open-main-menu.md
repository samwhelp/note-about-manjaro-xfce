---
title: 停用按鍵綁定「Super_L」開啟「Main Menu」
nav_order: 7022
has_children: false
parent: 如何
---


# 停用按鍵綁定「Super_L」開啟「Main Menu」




## 主題

* [前提](#前提)
* [如何設定](#如何設定)
* [如何停用](#如何停用)
* [如何恢復](#如何恢復)




## 前提

在「Manjaro Xfce」是透過「[~/.config/autostart/xcape.desktop](https://github.com/samwhelp/manjaro-xfce-adjustment/blob/main/sample/xcape/xcape.desktop#L7)」這個檔案，來執行「`xcape -e 'Super_L=Alt_L|F1'`」達成這個機制。




## 如何設定


### 如何停用

若要停用，執行下面指令，刪除「[~/.config/autostart/xcape.desktop](https://github.com/samwhelp/manjaro-xfce-adjustment/blob/main/sample/xcape/xcape.desktop#L7)」這個檔案。

``` sh
rm -f ~/.config/autostart/xcape.desktop
```


### 如何恢復

若要恢復，執行下面指令，恢復「[~/.config/autostart/xcape.desktop](https://github.com/samwhelp/manjaro-xfce-adjustment/blob/main/sample/xcape/xcape.desktop#L7)」這個檔案。

``` sh
cp /etc/skel/.config/autostart/xcape.desktop ~/.config/autostart/xcape.desktop
```
