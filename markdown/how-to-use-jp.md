<!-----
title: "SussyRaider 使い方ガイド"
----->
# 〜SussyRaider 使い方ガイド～

### 表示がちょっと見やすい版は[こちら](https://hackmd.io/@hIcQaeazRBmc_QUFj5HjlQ/BJz0vOuiF)

[:warning:] 現在Beta版の為モジュールがJoin/Leaver、Spammerしか無いです  
  今まであった機能を使いたいなら旧型を使おう

![](https://cdn.upload.systems/uploads/DAZQJDDk.png)


- このガイドはSussyRaiderの使い方を理解できない馬鹿の為にあります
- このガイドの最終更新は [2022/1/5 18:42 PM JST] です
- BruhTea#4000

## 前提条件
- SussyRaiderは**Windows10,64bit**環境でのみ動作確認、サポートを行っています
    - 他バージョンのWindowsでは正常に動かない場合があります(**あくまで可能性です**)
    - Windows10,64bit環境以外での動作は一切保証されません
- 高速なインターネット回線 (上り、下り50Mbpsほどあれば良い)
- スマートな脳
- トラブルに遭っても自分で解決しようとする力

## 必要な物
- Windows10 64bitが搭載された十分な性能を持つパソコン
- Discord Token
- 質の高いプロキシ

## アカウントの作成&ログイン
SussyRaiderは使うときにアカウントを作成する必要があります（初回のみ）  
1. まず[公式サーバー](https://discord.gg/Cdee9PTRg8)の`#hwid-issue`からチケットを作成し、Devたちに殴り込んでライセンスキーを入手します
2. ライセンスキーが手に入ったら、[SussyRaiderの登録ページ](https://sussyraider.cc/register)でアカウントを登録します  
   ライセンスキーを一番最後の場所に入れてください  
   ![register sample](https://i.imgur.com/sK7Kfad.png)
3. Dev達が疲弊するので、登録できたら殴り込みに行ったチケットをcloseしましょう
4. SussyRaiderを起動し、`userid`に貴方の設定したユーザー名、`password`にあなたのパスワードを入れて、`LaunchSussy`を押してください
5. SussyRaiderが起動します

## モジュールの操作方法

### プロキシやtokenの設定 (settings)
- 設定  
  基本的にSussyRaiderは先にプロキシをロードし、その後にTokenをロードします  
  スクリーンショットのように、使用するプロキシのタイプを選び、`Use Proxy`にチェックを入れ、プロキシをチェックし、最後にtokenをロードします。

![](https://cdn.upload.systems/uploads/Afq8D4Af.png)

Set Delayを使用することで遅延を設定できます。Delay 1 = 1秒の遅延  
これはApply を押すことで適用されます。

![](https://cdn.upload.systems/uploads/bScI5V2R.png)

[:x:] **Tokenをロードする前に Use Proxyにチェックを入れてください  
最悪の場合貴方のIPがDiscordにより規制されます**
- 少数tokenの場合(1~5個まで)ならなしでも大丈夫ｶﾓ

![](https://cdn.upload.systems/uploads/WM01FKhQ.gif)

### 入室/退室 (Join/Leave)
ボットをサーバーに入室させる場合、`InviteLink` へ招待を入れます  
招待を入れたら、左のタブの`SelectALL`を押すか、使用するtokenを選択します  
tokenの選択を終えた後、 `Join` を押すとボットの入室が始まります  

メンバースクリーニングの回避をするには、`Bypass  Member Screen`にチェックを入れ、サーバーIDを入れてから入室させます  
Tokenを退室させる場合は、 `ServerID` へサーバーのIDを入れます  
`Leave` を押すとサーバーからボットが退室します

![](https://cdn.upload.systems/uploads/oiBLQd1n.gif)

### サーバー内スパム (Spammer)
`ServerID`へスパム対象のサーバーのIDを入れ、`ChannelID`にはスパム対象のチャンネルのIDを入れます

#### 各種ボタン等の説明
┣ All Ping : サーバー内に居る全てのメンバーへメンションを飛ばします。対象のサーバーが1000人+の場合オンラインメンバーのみとなります  
┣ Spam to All Channel : サーバー内の発言可能な全てのチャンネルへスパムを行います  
┣ Random String : スパムする文章の最後へランダムな文字列を入れます  
┣ RateLimitFixer : レートリミットを掛けられた時、レートリミットが終わるまでリクエストの送信を一時停止します  
┃  
┣ Mention : All Pingでメンションする人数の設定を行います。All Pingを有効化しているときのみ動きます  
┗ SpamMessage : スパムする文章をここに入力します

Spamをする場合、
`Content`へメッセージを入れ、`Add Content`を押し、contentを
追加します(これは複数個追加可能)  
`Spam Start`でスパムを開始し、もしAll Pingが有効な場合メンバーの取得を行ってからspamを開始します  
`EndSpam`でスパムを停止

[:warning:] All Pingは不安定な為、動かない場合があります。一度停止してからもう一度開始すると動く場合があります

![](https://cdn.upload.systems/uploads/vPXswbzC.gif)

### 通報スパム (ReportSpam)
DiscordのAPIの通報スパムを行えます。[ここ](https://support.discord.com/hc/en-us/requests/new)からの通報では無いので気をつけてください。
`ServerID`にサーバーのID、`ChannelID`にチャンネルのID、`MessageID`にメッセージのIDを入れてください
#### ReportType(通報の理由)
┣ Illegal Content (違法なコンテンツ、二次元のロリ画像なども通る)  
┣ Harrasment (嫌がらせ等)  
┣ Spam or Phishing Links (スパム、又はフィッシングサイトへのリンク等)  
┣ Self harm (自殺行為等)  
┗ NSFW Content (NSFWチャンネルでないとこでのエロコンテンツなど)

一番上の`ReportSpam`を押すことで通報を開始できます。

### ニックネーム/アバター変更 (Nick/Avator)
ボットのニックネームやアバターを瞬時に変更できます

- アバターを変更する場合、`Avator URL`へ画像リンクを入れ、`ChangeAvator`をクリックします
- ニックネームを変更する場合、`ServerID`へサーバーIDを入れ、`Nickname`へニックネームを入れ、ChangeNickをクリックします

### フレンド/DMスパマー (Friend/DM)
フレンド申請、又はDMをスパムできます

- フレンド申請をスパムする場合、`User`へ名前#タグ形式の物を入れ、`FriendSend`をクリックします

- DMをスパムする場合、`UserID`へユーザーIDを入れ、`SpamMessage`へスパムするメッセージを入れ、`DMSpammer`をクリックします

[:warning:] DMスパムはTokenの寿命を削りやすい為、多用しないほうが良い。

### VCスパマー (VoiceSpammer)
ボイスチャンネルへのスパムを行えます

[:heavy_check_mark:] VCスパマーを使用する前にSussyRaiderの実行ファイルと同じフォルダに`ffmpeg.exe`、`libopus.dll`が存在する事を確認してください


`Voice Channel ID`へVCのIDを入れ、`ServerID`へサーバーのIDを入れます  
`VoiceFile mp3`を選択して.mp3形式の音楽ファイルを選択します  
`VoiceSpammer`をクリックすることでVCにスパムされます  

### リアクションスパム (Reaction)
壊れてるから書けないンゴーー

### ボタンプッシャー (Btn Pusher)
Ticket Botなどのボタンを押すことができます

`Server ID`へサーバーID、`Channel ID`へチャンネルID、`Message ID`へメッセージIDを入れ、Sendを押します

[:warning:] このモジュールは不安定な可能性があります


## してはいけない事
- プロキシ無しで使用する事 (極少数ボットのみを使用する場合は大丈夫)
- DM、フレンドを送りまくる事
- 超長時間スパムをすること
- ボイススパムを100token～でする事 (お前のPCのCPU、ネットワークの使用率がすごくなるぞ！！)
- ボイススパムをやりまくること
## よくありそうな質問

- Q. プロキシって何？  
┗ A. あなたのIPが規制されない為の中継サーバーです。無料で配布されている物は大体ゴミですので買いましょう。オススメはProxyscrapeのプレミアムです

- Q. Tokenって何？  
┗ A. Discordのアカウントの全てと言っても過言では無い物です。詳しくは別の人に聞いてくれ書ききれん

- Q. All Ping有効化してスパム開始したんだけど、ずっと発言されないんだけど？ゴミツールか？おい？
┗ A. メンバーの取得などができていなさそうな場合は一度停止してから開始してみてください。(メンバーの取得ができている場合、`[+] Get <USERID>`とコンソールに出てきます)

- Q. OnlinerとかReaction使えないんだけど？  
┗ A. Onlinerについてはまだ実装されとらんしReactionは壊れてるって書いてんだろメクラボケ

- Q. スパム開始しても発言が確認できないんだけど？？  
┗ A. ボットがミュートされていないか、又は蹴られたりしていないか確認してください。また、サーバーの認証レベルに引っかかってる可能性があるので、確認してください

- Q. DM/フレンドが送られてないみたいなんだけど？  
┗ A. 相手がDM/フレンドを拒否している可能性が高いです

- Q. 入室させたのに勝手に抜けてるんだけど？  
┗ A. Vortex等のアンチレイドが働いた可能性が高いです。遅延を設定した後、再試行してください。

- Q. 退室できないんだけど？  
┗ A. プロキシ又はTokenが死んだ可能性があります

- Q. スパムしようとしたらKeyErrorとか出るんだけど？  
┗ A. Botが蹴られている、又はBanされている、そもそも入室させていない可能性が高いです

- Q. Rate Limit!とか出たんだけど？  
┗ A. Discordにレートリミットを掛けられています。普通の場合、数秒で解除されるため、あまり気にしなくてもよいです

- Q. メンバースクリーニングって何？  
┗ A. これです。
![](https://pbs.twimg.com/media/EpyO3E6VQAA3H9Q.jpg)

- Q. メンションとかできないんだけど。  
┗ A. 普通に @Nigger#1234 とかやってもできないよ  
    - ユーザーメンション: `<@userid>`
    - ロールメンション: `<@&roleid>`
    - チャンネル: `<#channelid>`

- Q. 404ってエラー出てspamできないんだけど何？！？！  
┗ A. サーバーIDとかチャンネルIDとか間違えてそうなので確認してください

- Q. どうやってtoken手に入れるの？
┗ A. 買うか作れ。

## その他Discordについてのガイド

### Tokenの抜き方

※このガイドはPC専用。

1.Discordを開いている画面で`Ctrl+Shift+I`を押す。
2.開発者ツールが開くので、コンソールタブへ行く。
3.コンソールタブを開いたら、以下のコードをコピー＆ペーストする。
```
window.webpackChunkdiscord_app.push([[Math.random()], {}, (req) => {for (const m of Object.keys(req.c).map((x) => req.c[x].exports).filter((x) => x)) {if (m.default && m.default.getToken !== undefined) {return copy(m.default.getToken())}if (m.getToken !== undefined) {return copy(m.getToken())}}}]); console.log("%cWorked!", "font-size: 50px"); console.log(`%cYou now have your token in the clipboard!`, "font-size: 16px")
```
4.クリップボードにtokenがコピーされる。


その他不明な箇所があったら、Discord内で気軽に質問してください
誰かが答えると思う、多分



