# データ管理とファイルシステムの基礎

## データ管理とは

**データ管理**とは、コンピュータが扱うデータを適切に保存・取得・維持するための機能のこと。  
これにより、ユーザーやアプリケーションが必要なデータを効率よく扱えるようになる

### 例：
- **ファイルシステム**：データをファイルとして管理する仕組み  
- **バックアップ**：データのコピーを取り、消失や破損に備える手段

---

## ファイルシステムとは

**ファイルシステム**は、データを「ファイル」という単位で管理する仕組みであり、ファイルやディレクトリを階層構造で整理する。  
この構造により、データの検索や管理が容易になる。

---

## 基本用語の解説

### ファイルとは

記憶装置（HDD、SSD、USBメモリなど）に記録された**情報のまとまり**です。  
「ファイル」という言葉には「書類」という意味も含まれており、実際の文書やプログラム、画像など様々なデータがファイルとして保存される。

---

### ディレクトリとは

**ファイルを整理・格納するための場所（入れ物）**です。  
多くのファイルをグループごとに整理するために使われる。

---

### ディレクトリとフォルダの違い

- **ディレクトリ**：UNIX/Linux系の用語  
- **フォルダ**：Windowsで一般的に使われる用語  

どちらも同じ概念を指しており、「ファイルを入れるための容器」としての役割を持ちます。見た目や呼び方が違うだけ。

---

## ファイルシステムの構造

ファイルシステムでは、**ツリー構造**でファイルやディレクトリを管理する。  
この構造により、階層的に情報を分類・整理できる。

- **ツリー構造**：1つのルート（根）から枝分かれする形で構成される構造  
- 各枝が**ディレクトリ**や**ファイル**にあたる

---

## 重要なディレクトリの用語

### ルートディレクトリ（`/`）

ファイルシステムの**最上位**にあるディレクトリ。  
すべてのファイルやディレクトリは、このルートから枝分かれしている。

---

### カレントディレクトリ

現在ユーザーが**作業しているディレクトリ**のこと。  
コマンドライン操作やプログラムの実行時に、このディレクトリを基準としてファイルの場所を指定する。

---

## パスとは

**パス**は、ファイルやディレクトリの**場所（位置）を示す文字列**。

### パスの表記ルール（4つの基本）

1. ディレクトリやファイルは `/`（スラッシュ）で区切る  
2. パスの先頭が `/` の場合、それは**ルートディレクトリからの指定**（絶対パス）  
3. カレントディレクトリは `.`（ドット）で表す  
4. 1階層上のディレクトリは `..`（ドット2つ）で表す  

---

## 絶対パスと相対パス

### 絶対パス（Absolute Path）

- **ルートディレクトリ**（`/`）から始まるパス
- どこにいても目的のファイルやディレクトリにアクセス可能

#### 例：
/home/user/documents/report.txt


---

### 相対パス（Relative Path）

- **カレントディレクトリ**を基準にしたパス
- より柔軟にファイルを指定できるが、現在のディレクトリによって変わる

#### 例：
./documents/report.txt ../shared/image.jpg


---

## まとめ

- **ファイルシステム**はデータをファイル単位で管理し、階層的に整理する仕組み  
- **パス**はファイルの場所を示すために使い、絶対パスと相対パスが存在する  
- 正確にパスを使い分けることで、効率的にファイル操作が可能になる

---

