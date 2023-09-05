# counter_app

## 参考
https://github.com/rrousselGit/riverpod/tree/master/examples/counter

## このリポジトリの目的
- チュートリアルを振り返ることで、基礎的な状態管理の仕組みの理解を深める。
- 清書をしていきながら、RiverPodの導入について理解する。


## 学んだこと
- dartのビルド時にビルドできるプラットフォームの対象を選べるが、後から追加するのは結構手間だし、ドキュメントがあまりないので、最初に全部入りでビルドしておいたほうが良い。
- main.g.dart riverpod_generatorの生成物。`flutter pub run build_runner build`で生成される。(仕事上では現在利用しない。)
  - https://zenn.dev/riscait/books/flutter-riverpod-practical-introduction/viewer/riverpod-generator
- このアプリでは、データを一時的に保存し、不要になったら削除を自動で行う必要がある。そのため、`StateNotifier`を利用する。
  - おそらく、stateは、Reactでいうところ、propsみたいなもんっぽい。

## 業務で使えそうなポイント
- サクッと動かして、ぬるぬる遊ぶにはちょうど良さそう。
- UIもそんなに難しくないので、これで個人のサイトとか作ってみても良き。
- 業務で、使うには、Hiveでのキャッシュの保存や、APIのデータをどう格納するかっていう問題は解決できないので、もう少しチュートリアルを進めてみる。

