# このサイトについて

For full documentation visit [mkdocs.org](https://mkdocs.org).

会社で使っているコンフルみたいなサイトが自分用に欲しかったので作ってみました。
ページをMKDocsで作成し、GItHubPagesで公開しています。


## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs help` - Print this help message.

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.

### 作業時メモ
    [個人イントラサイトを作成する]

    あんどうめぐみさんのサイトがみやすくて良い感じだったのでGitHub Pagesを使用することにした。

    ■イントラサイトとは
        イントラサイトとは、企業や組織などの社内向けLANのサーバ上に構築された、業務向けのWebサイトのことである。

    ■イントラサイトの種類
        ■cell3dさんが使用しているサービス
            詳細不明。なんらかのイントラサイトらしい。
            https://twitter.com/cell3d/status/1194917383606980608

        ■あんどうれみりあさんが使用しているサービス
            GitHubPages
            https://fereria.github.io/reincarnation_tech/11_PySide/01_PySide_Basic/00_Tutorial/01_start/

        ■探してみたイントラサービス
            hugo
                https://twitter.com/piris314
                https://twitter.com/nananaoyamama/status/1193378788307959808
            Word Press

    ■参考ページ
        【GitHubPages】GitHub.ioで自己紹介ページを作りました
        https://qiita.com/ryokosuge/items/f929821ba5ae9ba2c32b
    ■アカウントを作成する
    ■リポジトリを作成する
    ■gitHub Desktop　からローカルにクローンする
    ■ページを確認する
        https://github.com/3str6/3str6.github.io
        https://3str6.github.io/

    ■テンプレートを探した
        はっきり流用できるものはなかった、jellykII とかRubyとか
        他にもwebpページのテンプレートを使うものとか

    □MKDocsがコンフルに似てて良さそう
        https://www.mkdocs.org/

    □MKDocsでサンプルページを作成する
        MkDocs：インストールから github pages へのデプロイまで
        https://www.kakistamp.com/entry/2019/08/31/154536
        カンタンにドキュメントが作れるmkdocsをはじめてみよう
        https://qiita.com/wamisnet/items/ed725d74f945f7c06b91
        MkDocsでドキュメント管理
        https://swfz.hatenablog.com/entry/2015/07/28/031712

    ■エラー解決用

    MkDocsによるドキュメント作成
    https://qiita.com/mebiusbox2/items/a61d42878266af969e3c

        GitHub Pages
        mkdocs には GitHub Pages にデプロイするコマンドが用意されています。
        GitHub でリポジトリを作成し、クローンして mkdocs のプロジェクトを構築して、以下のコマンドを実行します。

        mkdocs gh-deploy

        これだけでデプロイすることが出来ます。
        サイト：https://mebiusbox.github.io/MkDocsTest/
        ソース：https://github.com/mebiusbox/MkDocsTest
    
    ドキュメントをデプロイする
    https://www.mkdocs.org/user-guide/deploying-your-docs/

    [ mkdocsをgiHubPagesで表示できないエラーを解決する]
        ■サイトの情報をまとめる
            →2つあつめた
        □まず参考サイト①の手順通りにやってみる
        □次に公式ヘルプの手順通りにやってみる
        　→良い結果を得られなかった

        ---------------------------------------
        mkdocsファイルの作成
        mkdocs new sample01
        cd sample01
        mkdocs build
        mkdocs serve


        ---------------------------------------
        公式ヘルプのコマンドの結果
        C:\Users\Estragon\Documents\GitHub\3str6.github.io>mkdocs gh-deploy --config-file ../sample01/mkdocs.yml --remote-branch master
        INFO    -  Cleaning site directory
        INFO    -  Building documentation to directory: C:\Users\Estragon\Documents\GitHub\sample01\site
        WARNING -  Version check skipped: No version specificed in previous deployment.
        INFO    -  Copying 'C:\Users\Estragon\Documents\GitHub\sample01\site' to 'master' branch and pushing to GitHub.
        INFO    -  Your documentation should shortly be available at: https://3str6.github.io/3str6.github.io/

        ---------------------------------------
        mkdocsをリポジトリに登録する
        git init
        git add .
        git commit -m "first commit"
        git push -u origin mastergit remote add origin https://github.com/kakisoft/sample01.git
        git pull origin master

    □mkdocsを編集する
    VS CodeでMarkdownをプレビューするには？
    https://www.atmarkit.co.jp/ait/articles/1804/20/news030.html
    キーボード：［Ctrl］＋［K］→［V］
    	
    mkdocsを設定する
    https://fereria.github.io/reincarnation_tech/10_Programming/99_Documentation/00_mkdocs_setting/
