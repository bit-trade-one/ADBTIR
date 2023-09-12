# ADBTIR Bluetooth接続式赤外線送信モジュール
### [Q&A](FAQ.md)  
### [製品HP](https://bit-trade-one.co.jp/adbtir/)  


## 目次

### [使用用途・参照項目](#使用用途参照項目-1)

### [1.USB接続受信ツール使用方法](#1usb接続受信ツール使用方法-1)  
- [ダウンロード](#usb接続受信ツールダウンロード)
- [使用方法](#使用方法)
- [ファームウェアアップデート方法](#ファームウェアアップデート方法)

### [2.Bluetooth動作確認アプリ使用方法](#2bluetooth動作確認アプリ使用方法-1)
- [ダウンロード・準備](#ダウンロード準備)
- [A.本体に保存されている赤外線データの送信手順](#a本体に保存されている赤外線データの送信手順)
- [B.赤外線データの書き込み&送信手順](#b赤外線データの書き込み送信手順）
- [C.赤外線データの本体保存手順](#c赤外線データの本体保存手順)
- [D.コマンド作成](#dコマンド作成)

### [3.BluetoothBLE接続方法](#3bluetoothble接続方法-1)
- [BLE Scanner使用方法(Android)](#ble-scanner使用方法android)

### [4.ADBTIR-Bluetooth通信仕様](#4adbtir-bluetooth通信仕様-1)


---

## 使用用途・参照項目

系統図
<img src="images/fb4dbf4a6036cd47582173cf3fbb565db38f2ef89dfe7a29e0bb056e2c24a352.png"
        alt="ADBTIR系統図" width="800px">   

- USB接続で受信ツールを用いた赤外線受信信号の記録・送信  
   - [1.USB接続受信ツール使用方法](#1usb接続受信ツール使用方法-1)    
    
- Bluetooth動作確認アプリ・お客様の自作アプリを用いたBluetoothトリガによる赤外線信号制御  
   - [2.Bluetooth動作確認アプリ使用方法](#2bluetooth動作確認アプリ使用方法-1) 
   - [（1.USB接続受信ツール使用方法(赤外線信号の本体記憶))](#1usb接続受信ツール使用方法-1)   
   - [4.ADBTIR-Bluetooth通信仕様]()


- BluetoothBLT接続によるお客様の自作アプリからの赤外線信号制御
   - [3.BluetoothBLE接続方法](#3bluetoothble接続方法-1) 
   - [(1.USB接続受信ツール使用方法(赤外線信号の本体記憶))](#1usb接続受信ツール使用方法-1)  
   - [4.ADBTIR-Bluetooth通信仕様](#4adbtir-bluetooth通信仕様-1)



# 1.USB接続受信ツール使用方法

## USB接続受信ツールダウンロード
赤外線信号記憶・送信テストが可能です。  
ダウンロード・展開してお使いください。  
  
・設定ツールv100 __[【クリックでダウンロード】](https://github.com/bit-trade-one/ADBTIR/releases/download/V1/ADBTIR_BT_IR_Adapter_Recv_CT.exe)__
  
---

## 使用方法

ソフトを起動するとこの様な画面が表示されます。  
![picture 11](images/0c00f11942bb8c77f157db0d8f1670718aeeb3bc3311df57e470a11792d65eca.png)  

ADBTIRをPCと接続すると操作できるようになります。  
![picture 12](images/0aad1480b6893f336a37b122b6d9a5117d3c8ed346703398f81b4d2f28b89c7f.png)  

各種使用方法は以下をご参照ください。  
![picture 18](images/5a56f2d1dfa0ac845598e8e9831b94b08dd3a47bf1b6513847114e863d65a151.png) 


### ファームウェアアップデート方法  

現在公開されているファームウェアは無いため不要です。

>ファームウェアはハードウェアの中に書き込まれているソフトウェアのことを指します。  
>不具合修正や機能追加された新しいファームウェアが公開された際、  
>ファームウェアをアップデートすることで新しい機能が使用できます。  

<!--
1．ファームウェア書き込みツールを以下よりダウンロード・PCの任意の場所に保存します。  

[ファームウェア書き込みツール(最新v100)ダウンロードリンク](ここにURLを入力)



2.保存したファイルを展開してファームウェア書き込みツールを起動します。  
![image](ここにURLを入力)

3．設定ソフトの右下より本体をブートモードにすることも可能です。  
![image](ここにURLを入力)

4．Updateボタンを押すと書き換えが始まり、  
![image](ここにURLを入力)
「Verification successfull」が表示されれば完了です。  
![image](ここにURLを入力)

5．ADBTIRをパソコンのUSBコネクタから一旦取り外し、再度接続してお使いください。  
  -->




---

# 2.Bluetooth動作確認アプリ使用方法
 
 ### ダウンロード・準備  

  1.ADBTIR_BTIRAdapter.exeをダウンロード・起動します。

  ADBTIR_BTIRAdapter.exe __[【クリックでダウンロード】](https://github.com/bit-trade-one/ADBTIR/releases/download/V1/ADBTIR_BTIRAdapter.exe)__

  2 Bluetooth接続を行います。  
    PCと本機器のBluetoothペアリングを済ませた上で  左側の接続項目のPortNo.にてCOMポート番号を選択します。  
    本機器に割り当てられたCOMポート番号はWINDOWSのデバイスマネージャー等で確認できます。  
    その後、接続ボタンを押すと接続が完了します。  
   ![picture 3](images/23483f9e7d07415c0bdf3ae4e24d2d6191b179bfa9883470145ce9e500aa7fa3.png)  


### A.本体に保存されている赤外線データの送信手順  
  ADBTIR_BT_IR_Adapter_Recv_CT.exe等で本体に保存した赤外線信号を送信できます。  
  記憶させる方法は[1.USB接続受信ツール使用方法](#1usb接続受信ツール使用方法-1)を参照してください。  

  1 赤外線送信より、赤外線送信No.を選び、送信コマンドを押すと送信できます。
  ![picture 4](images/66a1d8a0ee271be15f0262292b610ec3a5fd5f37013ff4d718bb13fd5f17b9aa.png)  


### B.赤外線データの書き込み&送信手順

  1 赤外線データを準備します。  
  ADBTIR_BT_IR_Adapter_Recv_CT.exe(受信ツール,USB接続で通信)を起動し、赤外線データを取得します。  
  「記録開始」ボタン、「記録停止」ボタンで赤外線リモコンコードを記録し、「クリップボードにコピー」ボタンで赤外線データをクリップボードに取得できます。 
  ![picture 2](images/f1e9b65d86af8c4f662378d654dd890cdf7e1b7b5c73b2976188b4b72b0ff558.png)  


  2.右側の赤外線データ書き込み＆ 送信/保存から1.でコピーした赤外線データを貼り付けてください。  
  No.の選択、書き込み開始コマンド、書き込みコマンドを押すと書き込みが完了します。
  ![picture 6](images/04ae9b43066fe8709f747f127ffcb83ca5eea0ee1dd86755f5278b94c1f02f71.png)  

  3.赤外線データの送信手順  
   No.の選択、送信コマンドを押します。
   ![picture 7](images/e89eaf71231f597d6f853788437e6fef42df49c2a8eb753a9ed71be5116d392f.png)  

### C.赤外線データの本体保存手順  
  1 赤外線データを準備します。 (B-1参照)   
  2 右側の赤外線データ書き込み＆ 送信/保存から1.でコピーした赤外線データを貼り付けてください。  
  No.の選択、保存コマンドを押すと書き込みが完了します。  
  ![picture 9](images/86e7ccc8a2dbdb1976788883e5a2fc22affcffbfee1ab281ac04e0735287d40c.png)  


### D.コマンド作成
書き込まれた赤外線情報をもとに各種コマンドを書き出すことができます。
アプリ開発の際などにご利用ください。
![picture 10](images/d3e9b81eb1f61df76961849eacdf0ed443536b685c4141aec30972957ca5800d.png)  

詳細につきまして[4.Bluetooth通信仕様](#4adbtir-bluetooth通信仕様-1)もご確認ください。

---

# 3.BluetoothBLE接続方法

自作アプリを作成していただく他、接続の確認等であれば「BLE Scanner」の使用も可能です。

## BLE Scanner使用方法(Android)

1.Google Playより「BLE Scanner」をインストールします。  
<img src="images/4c32c00b993a028b5a1ac2bebbc866eeeac8fdd488a12c64f496f5dc777675d4.png"
        alt="picture 21" width="320px">   

2.BLE Scannerを起動し、「RN4678-」から始まる機器と接続します。  
<img src="images/8814c43194051dbb1cca33e14d8a5964358b79670955ef79eb49995045a498fb.png"
        alt="picture 22" width="320px">   


3.接続し様々な情報が確認できます。  
<img src="images/869ecccc50dea8d96ab4278c2a62551b698634ba3823fc85aa85b49bfa9ab761.png"
        alt="picture 23" width="320px">  

詳細につきまして[4.Bluetooth通信仕様](#4adbtir-bluetooth通信仕様-1)もご確認ください。

---
# 4.ADBTIR-Bluetooth通信仕様

以下からご確認いただけます。  
[ADBTIR-Bluetooth通信仕様(PDF)](https://github.com/bit-trade-one/ADBTIR/blob/main/Documents/ADBTIR%E9%80%9A%E4%BF%A1%E4%BB%95%E6%A7%98R01_20230728.pdf)

---

