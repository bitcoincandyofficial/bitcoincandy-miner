# 挖矿中文教程


1.获取钱包地址

可以通过以下几种方式获取
(1)各大交易所注册并获取CDY地址地址(CoinEX,btc-alpha等，最新的交易所支持请关注官网 https://cdy.one/)。
（CoinEX交易所注册地址 https://www.coinex.com/account/signup?refer_code=p3udv ）

(2)手机用户下载bitpie轻钱包，币种切换到CDY(客户端左上角选择币种)，地址： http://bitpie.com/

(3)下载我们的全节点钱包运行并获取钱包地址(https://github.com/bitcoincandyofficial/bitcoincandy/files/1707921/bitcoincandy-windows-exe.zip)




2. 根据你电脑型号选择合适的挖矿程序 

[下载 Windows  nVidia 挖矿程序](https://raw.githubusercontent.com/bitcoincandyofficial/bitcoincandy-miner/master/BitcoinCandy-nVidia.miner.0.3.4b.windows.zip)

[下载 Linux  nVidia 挖矿程序](https://raw.githubusercontent.com/bitcoincandyofficial/bitcoincandy-miner/master/Bitcoin-Candy-nVidia.miner.0.3.4b.Linux.Bin.zip)

[下载 Windows  AMD 挖矿程序](https://raw.githubusercontent.com/bitcoincandyofficial/bitcoincandy-miner/master/Claymore.s.BitcoinCandy.AMD.GPU.Miner.v12.6.zip)

[下载 Linux  AMD 挖矿程序](https://raw.githubusercontent.com/bitcoincandyofficial/bitcoincandy-miner/master/Claymore.s.BitcoinCandy.AMD.GPU.Miner.v12.6.-.LINUX.zip)


3.使用步骤1中获取的钱包地址替换挖矿脚本程序中的钱包地址，运行挖矿程序一般运行脚本程序(windows下start-CDY.bat或linux下start-bitcoin-candy.sh)  
如脚本start-CDY.bat中

miner --server pool.cdy.one --user CPH3VKnSbSgYgyBi5gqm35phEBMDfVhnaF.MyWorker --pass x --port 3857

请将CPH3VKnSbSgYgyBi5gqm35phEBMDfVhnaF替换为自己的CDY钱包地址，修改后直击双击脚本运行即可。


注意：windows系统下如果要直接运行“.exe”程序，N卡请在“miner.cfg”文件中修改钱包地址(矿池地址，端口号使用默认即可)，A卡则是修改config.txt。

4.注意

(1)请根据您电脑的型号选择正确的版本.

(2)确保你的显卡驱动是最新的（非最新容易出现闪退问题）.

(3)部分杀毒软件会将挖矿程序列为病毒，请将挖矿程序添加到杀毒软件的白名单或关闭杀毒软件.

(4)如无法定位挖矿程序无法正常启动的问题，可在当前目录打开命令行，运行挖矿脚步或程序查看错误信息提示。

(5)了解更多详情可参考文档 BItcoinCandyMiningReadme.docx 或 BitcoinCandy挖矿说明.docx


5.其他挖矿客户端
其他挖矿客户端包括DTSM和Bminer,亲测过Bminer，挖矿速度提升7%左右。

[Bminer挖矿客户端下载](https://www.bminer.me/releases/)
 
Linux
修改mine.sh脚本，示例如下：
#!/bin/sh

#Change the following address to your CDY taddr.  将如下地址改成你的CDY钱包地址

ADDRESS=CSZnk6KoMoEwHmveF3KcyRfEWsZfZ3dgEU

#你的矿工名myworker，可随意修改

USERNAME=$ADDRESS.myworker 

#修改矿池地址

POOL=pool.cdy.one:3857
SCHEME=stratum

./bminer -uri $SCHEME://$USERNAME@$POOL -api 127.0.0.1:1880

修改后运行mine.sh 


Windows
修改mine.bat  
@echo OFF

REM Change the following address to your Zcash taddr.

#Change the following address to your CDY taddr.  将如下地址改成你的CDY钱包地址
SET ADDRESS=CSZnk6KoMoEwHmveF3KcyRfEWsZfZ3dgEU

#你的矿工名myworker，可随意修改

SET USERNAME=%ADDRESS%.myworker 

#修改矿池地址

SET POOL=pool.cdy.one:3857

SET SCHEME=stratum

START "Bminer: When Crypto-mining Made Fast" bminer.exe -uri %SCHEME%://%USERNAME%@%POOL% -api 127.0.0.1:1880

修改后运行mine.bat


# bitcoincandy-miner
How to run a bitcoincandy miner program?

1.Get your own wallet address

There are several ways to gain your own CDY wallet address.

(1)Sign up for a digital coin exchange and acquire a CDY wallet address  (such as CoinEX, btc-alpha, for more supported exchange, go to https://cdy.one)
(you can sign up for CoinEX by following link: https://www.coinex.com/account/signup?refer_code=p3udv)

(2)Download Bitpie Mobile phone wallet, open this app and change your coin to CDY(at upper-left corner), and get a CDY address.
(download Bitpie app at http://bitpie.com/).

(3)run our full node wallet and get an address.(https://github.com/bitcoincandyofficial/bitcoincandy/files/1707921/bitcoincandy-windows-exe.zip)




2. Choose the right edition miner program to download according your computer 

[Download Windows CDY nVidia Miner](https://raw.githubusercontent.com/bitcoincandyofficial/bitcoincandy-miner/master/BitcoinCandy-nVidia.miner.0.3.4b.windows.zip)

[Download Linux CDY nVidia Miner](https://raw.githubusercontent.com/bitcoincandyofficial/bitcoincandy-miner/master/Bitcoin-Candy-nVidia.miner.0.3.4b.Linux.Bin.zip)

[Download Windows CDY AMD Miner](https://raw.githubusercontent.com/bitcoincandyofficial/bitcoincandy-miner/master/Claymore.s.BitcoinCandy.AMD.GPU.Miner.v12.6.zip)

[Download Linux CDY AMD Miner](https://raw.githubusercontent.com/bitcoincandyofficial/bitcoincandy-miner/master/Claymore.s.BitcoinCandy.AMD.GPU.Miner.v12.6.-.LINUX.zip)

3.Replace the wallet address in your miner's script(for windows, it's start-CDY.bat; for linux, it's start-bitcoin-candy.sh) with the address you acquire at step 1.

e.g, in start-CDY.bat: miner --server pool.cdy.one --user CPH3VKnSbSgYgyBi5gqm35phEBMDfVhnaF.MyWorker --pass x --port 3857

Replace CPH3VKnSbSgYgyBi5gqm35phEBMDfVhnaF with your own wallet address. Then save the file and double-click to run it.

4.notice

(1)Make sure you download the right edition program.

(2)Make sure  your graphics driver  is the newest(otherwise, unexpectedly quits will happen).

(3)Some anti-virus software will consider the miner program as a virus.You should add the software to whitelist or turn off the anti-virus software first.

(4)Open your miner by command line in your current directory when encountering a problem and you are not sure what it is.

(5)To get more detail instruction,see the BItcoinCandyMiningReadme.docx or BitcoinCandy挖矿说明.docx

5.Other mining clients
Other Mining clients include DTSM and Bminer,we have tested Bminer and we can get around 7% extra hash power。

[Download Bminer](https://www.bminer.me/releases/)
 
Linux
Edit mine.sh, see the following sample：
#!/bin/sh

#Change the following address to your CDY taddr.  

ADDRESS=CSZnk6KoMoEwHmveF3KcyRfEWsZfZ3dgEU

#change your worker name. 

USERNAME=$ADDRESS.myworker 

#Change your pool address

POOL=pool.cdy.one:3857
SCHEME=stratum

./bminer -uri $SCHEME://$USERNAME@$POOL -api 127.0.0.1:1880

Run mine.sh 


Windows
Edit mine.bat  
@echo OFF

REM Change the following address to your Zcash taddr.

#Change the following address to your CDY taddr.  

SET ADDRESS=CSZnk6KoMoEwHmveF3KcyRfEWsZfZ3dgEU

#change your worker name.

SET USERNAME=%ADDRESS%.myworker 

#Change your pool address

SET POOL=pool.cdy.one:3857

SET SCHEME=stratum

START "Bminer: When Crypto-mining Made Fast" bminer.exe -uri %SCHEME%://%USERNAME%@%POOL% -api 127.0.0.1:1880

Run mine.bat


Writen for pascal gpus but works on cards with at least 1Gb memory, and Compute Capability 3 and higher.
Miner contain dev fee 1%.

History:
Version 0.0.1 - CDY
- Added support for Bitcoincandy


