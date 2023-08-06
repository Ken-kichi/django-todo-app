# django-todo-app

初心者向けの Todo アプリ（Django）
[django-todo-app]

## 概要

このプロジェクトは、Django を使用して作成したシンプルな Todo アプリです。Todo アプリは、ユーザーがタスクを作成、更新、削除できるようになっています。

## 動作環境

このアプリケーションは、以下の環境で動作確認を行っています。

- Python 3.10.4
- Django 4.2.4

## インストール

1. Python をインストールしていない場合は、[Python の公式ウェブサイト](https://www.python.org/downloads/)からインストーラーをダウンロードし、インストールしてください。

2. Django をインストールします。ターミナル（コマンドプロンプト）を開き、次のコマンドを実行してください：

```bash
pip install Django
```

3. リポジトリをクローンします。

```bash
git clone https://github.com/Ken-kichi/django-todo-app.git
cd django-todo-app
```

## 実行方法

1. ターミナル（コマンドプロンプト）を開き、プロジェクトのルートディレクトリに移動します。

2. 仮想環境を作成します。

```bash
python -m venv .venv
```

3. 仮想環境を起動します。

```bash
source .venv/bin/activate
```

4. requirements.txt に書かれてあるライブラリを読み込みます。

```bash
python -m pip install -r requirements.txt
```

5. データベースをマイグレーションします。

```bash
python manage.py migrate
```

6. 開発用サーバーを起動します。

```bash
python manage.py runserver
```

4. ブラウザで以下の URL にアクセスします： `http://127.0.0.1:8000/todo/`

5. Todo アプリが表示されます。新しいタスクを作成したり、既存のタスクを更新したり、削除したりすることができます。

## アプリの機能

- タスクの一覧表示
- タスクの作成
- タスクの更新
- タスクの削除

## 注意事項

このアプリケーションは学習目的のために作成されており、実際のプロダクション環境での使用を意図していません。

### モデル

- `TodoTask`: タスクのモデルです。`title`（タイトル）、`description`（詳細）、`completed`（完了フラグ）の属性を持ちます。

### ビュー

- `todo_list`: タスクの一覧を表示します。
- `todo_create`: タスクの新規作成フォームを表示し、新しいタスクを作成します。
- `todo_update`: タスクの更新フォームを表示し、既存のタスクを更新します。
- `todo_delete`: タスクの削除確認画面を表示し、タスクを削除します。

### テンプレート

- `todo_list.html`: タスクの一覧を表示するテンプレートです。
- `todo_form.html`: タスクの作成と更新のためのフォームを表示するテンプレートです。
- `todo_confirm_delete.html`: タスクの削除確認画面を表示するテンプレートです。
