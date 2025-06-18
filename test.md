Gitとは？
Vesion Contorol Systemとは？
VCSには、どんなものがあるか？
Gitの歴史
だれがつくった？
メンテナーは日本人
リポジトリとは
リモート、ローカルリポジトリ
GitHubとは？
GitHub Webサービス
GitHubの類似サービス
GitHubでできること
GitHubにリポジトリをつくろう
自分のアカウントで新規のリポジトリを作成する

GitHub上で新しいリポジトリを作成して、開発をスタートしてみましょう。
READMEファイルを最初から作っておくと、cloneした後に中身を確認しやすくなります。

GitHub(https://github.com/)にログイン

右上の「+」 → 「New repository」をクリック

次のように設定

項目	設定内容
Repository name	repo-create-remote-start
Description	任意
Public / Private	任意
Add a README file	☑ チェックを入れる (作成する)
「Create repository」をクリック

作成したリポジトリをクローンして、ローカルにコピーを作成する

作成したリポジトリを、自分のPCにclone(複製)します。
ローカルでの編集や作業は、このcloneしたディレクトリ内で行います。

cd ~
git clone git@github.com:(ご自身のアカウント名)/repo-create-remote-start.git
ls -la # repo-create-remote-startディレクトリが確認できます。
ファイルを作成してみる

clone したディレクトリに移動し、新しいファイル local.txt を作成してみましょう。

cd ~/repo-create-remote-start
echo "これはローカルで追加したファイルです" > local.txt
ls -la
cat local.txt # local.txtが確認できます。