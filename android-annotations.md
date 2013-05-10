# OSO2013

subtitle
:   AndroidAnnotationsの紹介

author
:   @ryosms

date
:   2013/05/11

theme
:    rabbit

# 自己紹介

* [@ryosms](https://twitter.com/ryosms)
* 日本Androidの会 岡山支部
* 岡山Gitユーザ会([#okagit](https://twitter.com/search/realtime?q=%23okagit&src=typd))代表
	[http://okagit.github.io/](http://okagit.github.io/)
* OSO2013実行委員

# 自己紹介

* [@ryosms](https://witter.com/ryosms)

![](./images/best_tweet.png){:width='500' height='300' reflect_ratio='0.5'}

# OSO2012

* JavaFX on Android

:TODO 書く

# Android Annotations

* [http://androidannotations.org/](http://androidannotations.org/)
* Code Diet

# 使い方

* 公式読め
[https://github.com/excilys/androidannotations/wiki/Configuration](https://github.com/excilys/androidannotations/wiki/Configuration)
* ざっくり言えばannotation processorを有効に
* 指定されたAnnotation付けたらおｋ

# Annotation一覧（一部）

* @EActivity / @EFragment (components)
* @AfterViews / @ViewById (Injection)
* @Click / @TextChange (Event binding)
* 他にもまだまだあるよ！

詳しくは [https://github.com/excilys/androidannotations/wiki/AvailableAnnotations](https://github.com/excilys/androidannotations/wiki/AvailableAnnotations) 見れ

# 非同期処理

Androidでの非同期処理の歴史

# ～Android2.3

* UIスレッドで重い処理行うとANRが出るよ！
* 重い処理にはAsyncTask使おうね！
* UIと密なのがいやだったら自分でThreadとか駆使してね！

# Android4.0～

* 時代はAsyncTaskLoader
* LoaderではUI操作しないけど、CallbackするからUI操作が必要ならそこでやってね
* 1画面で複数のAsyncTaskLoader使いたいならinterfaceとか駆使してね！
　→例： [http://blog.livedoor.jp/ryosms/archives/5712827.html](http://blog.livedoor.jp/ryosms/archives/5712827.html)

Android 3.x？なにそれおいしいの？

# Android Annotationsの場合

* 非同期で実行するメソッドに@Background付ければおｋ
* UIの操作がやりたいなら@UiThread付ければおｋ
* あら簡単！

# まとめ

* 便利だよ
* 簡単だよ
* 今までの苦労はなんだったのか

※仕事でAndroid Annotations使ったら、Android初心者が「Webに載ってるサンプルコードとあまりにも違いすぎてわからん！」って発狂してたよ


# おしまい

* ご静聴ありがとうございました

![](./images/bell6.png){:width='300' height='300' reflect_ratio='0.5'}

