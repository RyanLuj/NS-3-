**#NS-3 環境建立**  
___
#NS-3 簡介  
● ns (network simulator) 包括 ns-1、ns-2 和 ns-3，是一系列離散事件網絡模擬器， 主要應用於研
究和教學。  
● ns-3 是一個 open source 的研究用網路模擬工具。  
___
**#NS-3 Installation Part1**  
● 安裝必要套件  
```
$ sudo apt install g++ python3 python3-dev pkg-config sqlite3 cmake
```  
● 下載 ns-3.35 壓縮檔  
```
$ cd && wget -c https://www.nsnam.org/releases/ns-allinone-3.35.tar.bz2
```
● 解壓縮至 home 資料夾  
```
$ tar -xvjf ns-allinone-3.35.tar.bz2
```
___
**#NS-3 Installation Part2**  
● 更改路徑至目標資料夾  
```
$ cd ns-allinone-3.35/ns-3.35/
```
● Configure the installation  
```
$ ./waf configure --enable-examples
```
● Build ns-3 installation  
```
$ ./waf
```
● Check the installation  
```
$ ./waf --run hello-simulator
```
___
**#NS-3 Installation Part2**  
![Image](https://github.com/user-attachments/assets/ecb42d5b-e78d-4f98-9d04-a78dfdfbc15a)
___

**#NS-3 可視化工具 NetAnim Installation**  
● 更改路徑至目標資料夾  
```
$ cd && cd ns-allinone-3.35/netanim-3.108
```
● Configure the build  
```
$ make clean
```
● Build NetAnim installation  
```
$ qmake NetAnim.pro
```
```
$ make
```  
● Execute NetAnim  
```
$./NetAnim
```
___
**#NS-3 可視化工具 NetAnim Installation**  
![Image](https://github.com/user-attachments/assets/da5df35d-7769-4943-8133-c7a740300aea)  
___
**#NS-3 Example**  
● 將 ns-3.35/examples/tutorial/first.cc 檔案複製至 ns-3.35/scratch 資料夾  
● build this example  
```
$ cd && cd ns-allinone-3.35/ns-3.35/
```
```
$ ./waf –run first
```
![Image](https://github.com/user-attachments/assets/effa162d-01d1-4cda-942d-18fd4707d602)   
___
**#NS-3 Example**  
![Image](https://github.com/user-attachments/assets/c2a1b3d8-f9d6-4a12-bb15-c7b3a74b111c)  
___
**#NS-3 Example**  
![Image](https://github.com/user-attachments/assets/a5c5c1cd-b3ea-49f8-bd5a-2f25a8c2f013)  
___
**#NS-3 Example**
![Image](https://github.com/user-attachments/assets/88263c7f-aade-4de6-a8af-eb9e8bfdcc8d)  
___
**#NetAnim Example**  
● 增加第22,77行程式碼，再重新 build 一次  
```
$ ./waf –run first
```
![Image](https://github.com/user-attachments/assets/3678f562-1fc1-4b78-a9d0-de19f70a1812)  
![Image](https://github.com/user-attachments/assets/12384e0e-0e5c-4764-aa31-0ad21b9f7f86)  
___
**#NetAnim Example**  
● first.xml檔案會生成在ns-3.35資料夾  
●開啟Execute NetAnim
```
$./NetAnim
```
● 載入 first.xml 檔
___
**#NetAnim Example**
![Image](https://github.com/user-attachments/assets/f9f4124b-0c3a-4af4-88c6-16be8b14d3e6)
![Image](https://github.com/user-attachments/assets/99494a2e-a76e-4498-a984-e3b62fd84369)





