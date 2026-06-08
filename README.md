# 基礎プログラミングII — 第9回 演習（2026-06-08）

**科目:** 基礎プログラミングII　**対象:** 2年生

---

## 手順

1. このリポジトリを **Fork** する（画面右上の「Fork」ボタン）
2. 自分のリポジトリをローカルに **Clone** する

```bash
git clone https://github.com/自分のユーザー名/kiso-prog2-09-0608.git
cd kiso-prog2-09-0608
```

3. `ex_write.c` から順に `/* TODO */` の部分を埋めてコンパイル・実行する
4. 全部終わったら **Push** する

```bash
git add .
git commit -m "演習完了"
git push origin main
```

5. GitHub で **Pull Request** を出す
   - タイトルは **自分の名前**（例：`山本周`）
   - base: `yamashu00/kiso-prog2-09-0608` ← `main`

---

## ファイル一覧

| ファイル | 難易度 | 内容 |
|---------|-------|------|
| `ex_write.c` | ★ | 名前・整数・小数をCSVに書く |
| `ex_read.c` | ★ | CSVを読み込んで表示する |
| `task1_log.c` | ★★ | 実行するたびに1行追記する |
| `task1_count.c` | ★★ | ログの行数を数える |
| `task2_max.c` | ★★★ | 最高気温の場所を探す |
| `task3_copy.c` | ★★★★ | CSVファイルをコピーする |

`ex_write.c` と `ex_read.c` は全員やること。  
`task1〜task3` は余った時間で挑戦してみよう。

---

## コンパイルと実行（例）

```bash
gcc ex_write.c -o ex_write
./ex_write
```

---

## 参考資料

授業資料（lesson-09-ref.md）を見ながら進めてよい。
