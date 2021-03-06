# C/C++ 言語 (Gitpod)
1. 環境構築 | Web IDEである　[Gitpod](https://www.gitpod.io/docs/getting-started)　の導入

2. Gitpod 導入
   - 環境構築を簡略化
   - os に依存しない C, C++ 環境を整えられるかどうか

3. C言語
   - basic
   - algorithm
4. C++
   - basic

   - CMake を使用して biuld
     - [CMake の使い方](https://qiita.com/shohirose/items/45fb49c6b429e8b204ac)
     - [CMake document](https://cmake.org/cmake/help/v3.22/guide/tutorial/A%20Basic%20Starting%20Point.html)
     - document.md 参照

## Gitpod
> https://www.gitpod.io/docs/getting-started
### 1. Repository に添付 -> Enter
- browser’s address bar に　->　`gitpod.io/#`

  - 例）
    ```
    gitpod.io/#https://github.com/gitpod-io/website
    ```
    - そうする事で browser 上で 添付した Repository 環境で Gitpod を使用できる

### 2. C言語の実行 file 作成

    # 実行file作成 : compile
    gcc -o <実行file名> file名.c

    # 実行
    ./<実行file名>
- working dirctory で compile & 実行

### 3. code format : .clang-format 作成

    # terminal で実行 : file作成
    clang-format -style=llvm -dump-config > .clang-format

    # clang-format : 変更
    IndentWidth: 4
- 拡張機能 : [clangd](https://marketplace.visualstudio.com/items?itemName=llvm-vs-code-extensions.vscode-clangd) install
- [Clang-Format Style](https://clang.llvm.org/docs/ClangFormatStyleOptions.html)

### 4. debug 拡張追加
- 拡張機能 : [C/C++](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools) install
