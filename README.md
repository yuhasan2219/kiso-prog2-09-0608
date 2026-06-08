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

3. 以下の順にコンパイル・実行して確認する（各ファイルの先頭コメントに手順あり）

   **① デモ（動かして確認するだけ）**
   ```
   step0_no_file.c  → step0_with_file.c
   step1_write.c    → step1_append.c
   step2_no_null_check.c → step2_with_null_check.c
   step3_no_fclose.c → step3_with_fclose.c
   step4_read_one.c  → step4_read_all.c → step5_all.c
   ```

   **② 演習（`/* TODO */` の部分を自分で埋める）**
   ```
   ex_write.c → ex_read.c
   ```

   **③ 発展（余った時間で挑戦）**
   ```
   task1_log.c → task1_count.c → task2_max.c → task3_copy.c
   ```

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

---

## printf / fprintf のフォーマット指定子

| 指定子 | 対応する型 | 意味 | 覚え方 |
|--------|----------|------|--------|
| `%s` | `char[]` / `char *` | 文字列 | **S**tring |
| `%d` | `int` | 10進整数 | **D**ecimal |
| `%c` | `char` | 1文字 | **C**haracter |
| `%f` | `float` / `double` | 実数 | **F**loating point |

```c
printf("%s は %d°C、湿度 %.1f%%\n", "教室", 25, 60.5);
//      %s       %d         %f
//       ↑       ↑           ↑
//      char[]  int         float
```
