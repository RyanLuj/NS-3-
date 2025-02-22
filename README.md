**#NS-3 環境建立**
#NS-3 簡介  
● ns (network simulator) 包括 ns-1、ns-2 和 ns-3，是一系列離散事件網絡模擬器， 主要應用於研
究和教學。  
● ns-3 是一個 open source 的研究用網路模擬工具。  

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
**#NS-3 Installation Part2**  
![Image](https://github.com/user-attachments/assets/ecb42d5b-e78d-4f98-9d04-a78dfdfbc15a)

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
./NetAnim
```
**#NS-3 可視化工具 NetAnim Installation**  
![Image](https://github.com/user-attachments/assets/da5df35d-7769-4943-8133-c7a740300aea)  
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
**#NS-3 Example**  
![Image](https://github.com/user-attachments/assets/7c59bd91-0e3a-4a52-b93d-1006f19fadfb)






