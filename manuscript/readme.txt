%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%
%		RTグループ修士論文テンプレート(英語)
%
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

%%% はじめに
本テンプレートはUbuntu (8.10で動作を確認) においてlatexコマンドを
用いてコンパイルすることを前提として作られています。
それ以外の環境の方はコンパイルできるように適宜変更してください。


%%% コンパイルの方法
分割コンパイルをしている。

メインファイルの末尾:
%%% Local Variables:
%%% mode: latex
%%% TeX-master: t
%%% End:

サブファイルの末尾:
%%% Local Variables:
%%% mode: latex
%%% TeX-master: "main" <- メインファイルへのパス
%%% End:

の記述によってmain.tex以外のファイルからもC-c C-cでコンパイルが可能。


%%% 使用パッケージ
% graphicx
画像を扱うためのパッケージ。
graphicの拡張版らしい。
こちらの使用が推奨されている。

% amsmath, amssymb
数式を扱うためのパッケージ。
amsmathがコアでamssymbは数学記号をサポートするらしいです。


%%% ファイル/ディレクトリ構成

% main.tex
本体。その他のファイルを\inputで読み込む。
\includeなどでも読み込めるが、コンパイルの
際のファイルの有無の確認などに際がある模様。

% chapter*.tex
各章のtexファイル。

% macros.tex
マクロとスタイルが混在しています。

% ref.tex
参考文献。

% acknowledgment.tex
謝辞。

% figure/*
各章で使用する画像を配置。

% thesis.sty
book.clsを利用する場合のスタイル変更。