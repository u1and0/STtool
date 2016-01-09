+ [keymap & mousemap & setting](#keymap)
+ [Theme](#theme)
+ [syntax settings](#syntax-settings)
+ [build series](#build-series)
+ [initial series](#initial-series)
+ [insert date](#insert-date)
+ [line series](#line-series)
+ [Enhanced text](#enhanced-text)
+ [package's sublime setting](#package)
+ [なんだこれ](#なんだこれ)










-----------------------------------------------------------------------


## keymap & mousemap & setting
* Preferences.sublime-settings
	主な設定version わかんない
* Default (Linux).sublime-keymap
* Default (OSX).sublime-keymap
* Default (Windows).sublime-keymap
	<UPDATE7.2>
	+ Auto pair \*
		select内を*でくくる
		他のAuto pairと異なり、何もない行に*を打ち込んだときは通常通り*が打たれる(項目として使われる*, 計算式として使われる*が必要だから)
	+ Auto pair ~
		打消し線~~が打たれる
	+ Auto pair  \` 
	<ver7.1>  
	- Auto-pair percent %の自動補完  
	- "ctrl+p","ctrl+w" ワークスペースの保存  
	- "ctrl+e","ctrl+f" evernote search_note  

* Default (Windows).sublime-mousemap
	<ver3.1>  
	+ expand selection to scope
	+ PageScroll
	+ soft undo & soft redo
	+ jump
	+ undo & redo
	+ Change tabs
	+ Select scope~~+ Select all~~

* Default (Windows).sublime-mousemap.txt
	sublimetext2から拾ってきたマウスマップのデフォルト  
	参考用なので拡張子が.txt  

* Default (Windows).sublime-mousemap
	ver3.1
	+ expand selection to scope
	+ PageScroll
	+ soft undo & soft redo
	+ jump
	+ undo & redo
	+ Change tabs
	+ Selct all

* Default (Windows).sublime-mousemap.txt  
	sublimetext2から拾ってきたデフォルト
-----------------------------------------------------------------------
## Theme
Tubnil_kai.tmTheme
Tubnil_kai.tmTheme.cache






-----------------------------------------------------------------------
## syntax settings
* C++.sublime-settings
* MQL4.sublime-settings
* HTML.sublime-settings
* Markdown.sublime-settings
* INI.sublime-settings
* Plain text.sublime-settings
* vbdotnet.sublime-settings





-----------------------------------------------------------------------
## build series
* batch.sublime-build
* html.sublime-build
* perl.sublime-build
* platex.sublime-build


-----------------------------------------------------------------------
## initial series
行頭に移動して所定の記号を入力するマクロ及びスニペット郡  
keymapで`ctrl+alt+/`で起動するように設定している  
コメントアウト//のみ`ctrl+/`で起動するようにしてある  
以下initialフォルダの中身  
* Comments (C++).tmPreferences
	mt4コメントアウトをC++のシンタックスと合わせた
* comment_out.sublime-macro  
	 `Enhanced textのコメント` アウト  
* comment_out_bat.sublime-macro  
	batchのコメントアウト  
* comment_out_vbnet.sublime-macro  
	VB.NETのコメントアウト  
* Default (Windows).sublime-keymap  
	ショートカットで起動できるように登録  
* initial_mark.sublime-macro  
	選択範囲を行ごとにキャレット分割して行頭にキャレット持ってきて以下のスニペット起動
* initial_at.sublime-snippet  
	@を挿入
* initial_dat.sublime-snippet  
	・を挿入
* initial_ket.sublime-snippet  
	引用符>を挿入
* initial_minus.sublime-snippet  
	ハイフンを挿入
* initial_plus.sublime-snippet  
	+を挿入
* initial_sharp.sublime-snippet  
	#を挿入
* initial_star.sublime-snippet  
	*を挿入
* initial_Wslash.sublime-snippet  
	//を挿入(コメントアウト)




-----------------------------------------------------------------------
## insert date
ページのトップにアンダースコア２つと今日の日付を入れる  
**package insertdate**が必要
* insertdate.sublime-macro



-----------------------------------------------------------------------
## line series
-,=,*,_を入力した後にtabキー押すとその文字を20字くらい打って線にしてくれる。  
中央にコメントも入れられる。  
* line_double.sublime-snippet
* line_single.sublime-snippet
* line_star.sublime-snippet
* line_under.sublime-snippet




-----------------------------------------------------------------------
## Enhanced text
自分用シンタックス。.txtや.md形式のファイルをより見やすくするために作った
* EnhancedTXT.sublime-settings
* EnhancedTXT.tmLanguage
* EnhancedTXT.YAML-tmLanguage

[UPDATE3.1]  
+ <>の色を緑に変更
	- 元々緑だった@は紫に変更
+ 項目番号の表示修正
	- 2桁以上の数字に対応できるようにした
	- 行頭だけではなく、先頭文字がスペースまたはタブでも色変え対象とした  
		{"match": "(\\s|^)\\d+\\.\\s",

[UPDATE3.0]  
+ MarkDown記法への対応  
	- [ライン]ハイフン2個以上並んだとき、以下を色変え  
	- [項目]+,-,*とスペース  
	- [数字項目]数字とドット  
	- [ボールド体]アスタリスク*2個のならびに囲まれた文字  
	- [イタリック体]アスタリスク*1個のならびに囲まれた文字  
	- [打ち消し文字]チルダ~2個のならびに囲まれた文字  
	- [コード]バッククォート\`内、及びバックォート\`以下  
	- [リンク]\(\)内のhttp,https以下の文字  
	- [見出し]シャープ#1個以上とスペースがついたとき以下の色変え  
+ カッコの修正  
	- シングル・ダブルクオート内の色変えの修正  
	- 色変えに対応したカッコのを増やした(飾りカッコや全角＜＞)  
	- 角カッコは2重以上でも色がつく  
+ その他  
	- @マーク以下の色変えは閉じ文字としてスペース2つ以上  
	- *マーク後にスペース入れなきゃ色変えしないようにした  
	- ブロックコメントアウト/*は削除  


## package's sublime setting
導入しているpackageのセッティング
* insert_date.sublime-settings
* Package Control.sublime-settings
* Side Bar.sublime-settings
* trailing_spaces.sublime-settings
~~* Evernote.sublime-settings~~		token含まれているからignore


## なんだこれ
* ST_csv_edt.sublime-macro







