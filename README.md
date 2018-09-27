# 挖矿中文教程


1.获取钱包地址

可以通过以下几种方式获取
(1)各大交易平台注册并获取CDY地址地址(CoinEX,btc-alpha等，最新的交易所支持请关注官网 https://cdy.one/)。
（CoinEX交易平台注册地址 https://www.coinex.com/account/signup?refer_code=p3udv ）

(2)手机用户下载bitpie轻钱包，币种切换到CDY(客户端左上角选择币种)，地址： http://bitpie.com/

(3)下载我们的全节点钱包运行并获取钱包地址(https://github.com/bitcoincandyofficial/bitcoincandy/releases/download/0.17.2/bitcoin-qt.exe)




2. 根据你电脑型号选择合适的挖矿程序(升级Equihash 144.5后，请使用旧挖矿客户端的用户及时下载以下新客户端)

[下载 Windows  nVidia 挖矿程序](https://github.com/bitcoincandyofficial/bitcoincandy-miner/raw/master/windows-Equihash_144_5-miner-nVidia.zip)

[下载 Linux  nVidia 挖矿程序](https://github.com/bitcoincandyofficial/bitcoincandy-miner/raw/master/EWBF_Equihash_144_5miner_v0.5.tar.gz)


部分使用旧驱动(cuda 8)的nVidia可尝试使用以下版本客户端。

[下载 Windows  nVidia cuda8 挖矿程序](https://github.com/bitcoincandyofficial/bitcoincandy-miner/raw/master/windows-Equihash_144_5-miner-nVidia-cuda%208.zip)

[下载 Linux  nVidia cuda8 挖矿程序](https://github.com/bitcoincandyofficial/bitcoincandy-miner/raw/master/EWBF_Equihash_144_5miner_v0.5_cuda_8.tar.gz)


AMD显卡使用以下版本客户端。

[下载 Windows  AMD 挖矿程序](https://github.com/bitcoincandyofficial/bitcoincandy-miner/raw/master/AMD_lolMiner_v043b_Win64.zip)

[下载 Linux  AMD 挖矿程序](https://github.com/bitcoincandyofficial/bitcoincandy-miner/raw/master/AMD_lolMiner_v043b_Lin64.tar.gz)


3.使用步骤1中获取的钱包地址替换挖矿脚本程序中的钱包地址


(1)Windows客户端

运行挖矿程序一般运行脚本程序(windows下run.bat或linux下mine.sh)  
如脚本run.bat中

miner  --algo 144_5 --pers CandyPoW  --server pool.cdy.one --port 3857 --user CSZnk6KoMoEwHmveF3KcyRfEWsZfZ3dgEU.myworker --pass x


请将CSZnk6KoMoEwHmveF3KcyRfEWsZfZ3dgEU替换为自己的CDY钱包地址，修改后直击双击脚本运行即可。


[nVidia挖矿教程](https://bitcointalk.org/index.php?topic=4466962.0)





(2)对于AMD挖矿客户端：

替换user_config.json 中的USER选项为自己的钱包地址

"USER" : "CSZnk6KoMoEwHmveF3KcyRfEWsZfZ3dgEU.lolMiner",
 
 
 windows 双击run_miner.bat运行
 
 linux 下运行run_miner.sh
 


4.注意

(1)请根据您电脑的型号选择正确的版本.

(2)确保你的显卡驱动是最新的（非最新容易出现闪退问题）.

(3)部分杀毒软件会将挖矿程序列为病毒，请将挖矿程序添加到杀毒软件的白名单或关闭杀毒软件.

(4)如无法定位挖矿程序无法正常启动的问题，可在当前目录打开命令行，运行挖矿脚步或程序查看错误信息提示。

(5)了解更多详情可参考







# Mining tutorial
How to run a bitcoincandy miner program?

1.Get your own wallet address

There are several ways to gain your own CDY wallet address.

(1)Sign up for a digital coin exchange and acquire a CDY wallet address  (such as CoinEX, btc-alpha, for more supported exchange, go to https://cdy.one)
(you can sign up for CoinEX by following link: https://www.coinex.com/account/signup?refer_code=p3udv)

(2)Download Bitpie Mobile phone wallet, open this app and change your coin to CDY(at upper-left corner), and get a CDY address.
(download Bitpie app at http://bitpie.com/).

(3)run our full node wallet and get an address.(https://github.com/bitcoincandyofficial/bitcoincandy/releases/download/0.17.2/bitcoin-qt.exe)




2. Choose the right edition miner program to download according your computer （upgraded as Equihash 144.5）

[Download Windows CDY nVidia Miner](https://github.com/bitcoincandyofficial/bitcoincandy-miner/raw/master/windows-Equihash_144_5-miner-nVidia.zip)

[Download Linux CDY nVidia Miner](https://github.com/bitcoincandyofficial/bitcoincandy-miner/raw/master/EWBF_Equihash_144_5miner_v0.5.tar.gz)

For those with cuda 8, use the folllowing miner:

[Download Windows CDY nVidia Miner](https://github.com/bitcoincandyofficial/bitcoincandy-miner/raw/master/windows-Equihash_144_5-miner-nVidia-cuda%208.zip)

[Download Linux CDY nVidia Miner](https://github.com/bitcoincandyofficial/bitcoincandy-miner/raw/master/EWBF_Equihash_144_5miner_v0.5_cuda_8.tar.gz)


For AMD graphic cards:

[Download Windows  AMD miner](https://github.com/bitcoincandyofficial/bitcoincandy-miner/raw/master/AMD_lolMiner_v043b_Win64.zip)

[Download Linux  AMD miner](https://github.com/bitcoincandyofficial/bitcoincandy-miner/raw/master/AMD_lolMiner_v043b_Lin64.tar.gz)




3.

(1)Nvidia miners

Replace the wallet address in your miner's script(for windows, it's run.bat; for linux, it's mine.sh) with the address you acquire at step 1.

e.g, in run.bat: miner  --algo 144_5 --pers CandyPoW  --server pool.cdy.one --port 3857 --user CSZnk6KoMoEwHmveF3KcyRfEWsZfZ3dgEU.myworker --pass x

Replace CSZnk6KoMoEwHmveF3KcyRfEWsZfZ3dgEU with your own wallet address. Then save the file and double-click to run it.


[nVidia Tutorial](https://bitcointalk.org/index.php?topic=4466962.0)


(2)AMD miners

Firstly, modify "USER" option in user_config.json 

"USER" : "CSZnk6KoMoEwHmveF3KcyRfEWsZfZ3dgEU.lolMiner",
 
replace CSZnk6KoMoEwHmveF3KcyRfEWsZfZ3dgEU with your own wallet address.

 
Next, double click run_miner.bat for windows; For linux, run run_miner.sh
 



4.notice

(1)Make sure you download the right edition program.

(2)Make sure  your graphics driver  is the newest(otherwise, unexpectedly quits will happen).

(3)Some anti-virus software will consider the miner program as a virus.You should add the software to whitelist or turn off the anti-virus software first.

(4)Open your miner by command line in your current directory when encountering a problem and you are not sure what it is.








