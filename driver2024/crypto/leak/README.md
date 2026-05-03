# leak

## 問題文
先月、日本の会社で大規模なBTCの不正流出が起きた。  
流出先となっているウォレットアドレスを答えよ。  
Flag形式: `Diver24{ウォレットアドレス}`  

## 難易度

easy / 100 point (211 Solves)

## 自分で解法を考える
README.mdの情報量が少なすぎるので、現実に起きたことではないか？
そこで、"bitcoin 2024 leak japan"と検索した
すると、DMM Bitcoinが2024年5月31日に不正流出したとのこと
おそらくこの件の流出先となっているウォレットアドレスを調べればいいのではないか？
北朝鮮ハッカー集団"TraderTraitor"の関連口座に流出したとのこと
Flag形式：`Diver24{TraderTraitor}` 

## 解法
<details>
<summary>クリックで表示</summary>
 
`btc leak may 2024` などとGoogleで調べると、5月31日にDMM Bitcoinが約3億ドル分のBTCの不正流出の被害に遭っていることが分かります。  
X（Twitter）で`dmm btc address`と調べると、まとめている[ポスト](https://x.com/lookonchain/status/1796789067499327649)があり、流出先となっているウォレットアドレスが記載されています。
また、このアドレスは[Binance News](https://www.binance.com/ja/square/post/2024-05-31-stolen-bitcoins-from-japanese-exchange-dmm-bitcoin-distributed-to-ten-addresses-8846900839153)など他のソースにも記載されているほか、[Whale Alert](https://whale-alert.io/transaction/bitcoin/975ec405ac9dc9fa5ab8009d94d6a1fe31dff8a8127ea90d023104e52754e4d7)からも確認できます。
**Diver24{1B6rJRfjTXwEy36SCs5zofGMmdv2kdZw7P}**
</details>

## 結果
不正解

## AIによるアドバイス
<details>
事件の特定までは合っていました。  
「日本の会社」「大規模なBTC不正流出」から、DMM Bitcoinの事件にたどり着けた点は良かったです。

不正解の原因は、答える対象を取り違えたことです。  
問題で求められているのは攻撃グループ名ではなく、流出先のウォレットアドレスでした。

`TraderTraitor` ではなく、BTCアドレス形式の値を答える必要がありました。

今後は、最後に「問題が求めている値の種類と、自分の答えが一致しているか」を確認するとよいです。

</details>

## 反省
アドレス=攻撃者のグループ名だと勘違いしていた。