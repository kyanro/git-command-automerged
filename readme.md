# 準備
git-automerged をパスが通った場所におく

# 使い方
`git automerged commit_hash`

*commit_hash* : HEAD, master, branch_name, cc2ef04, *etc...*

## *commit_hash* が merge commit だった場合
+ 親の一覧
+ auto merge が発生したファイル一覧
が出力される

例) masterがmerge直後の場合

	$ git automerged master
	Pearent 1 : cc2ef04a6311275da00ab1a886d9fb671f87763f
	Pearent 2 : 7edb43954e9b756cc3de5ba27ed98b592ea222f8
	 *AutoMerged filenames...
	auto_merged.txt
	auto_merged2.txt
	auto_merged3.txt
	auto_merged4.txt

## *commit*を省略した場合
+ HEAD が利用される

例) HEADがmerge直後の場合

	$ git automerged
	Pearent 1 : cc2ef04a6311275da00ab1a886d9fb671f87763f
	Pearent 2 : 7edb43954e9b756cc3de5ba27ed98b592ea222f8
	 *AutoMerged filenames...
	auto_merged.txt
	auto_merged2.txt
	auto_merged3.txt
	auto_merged4.txt
