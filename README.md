
  copilot-demo

  GitHub Copilot CLI のデモプロジェクト。Copilot CLI を使った提案受け取りや、README・ワークフローの動作確認を目的としています。

  概要

  このリポジトリは GitHub Copilot CLI（gh copilot）の動作確認用です。README の自動生成や CI ワークフローの検証に利用してください。

  前提条件

   - GitHub CLI（gh）がインストールされていること
   - Copilot 拡張が利用可能であること（必要に応じて gh extension install github/gh-copilot）
   - GitHub にログインしていること（gh auth login）

  使い方

   1. リポジトリに移動:
   cd C:\Users\kikir\copilot-demo
   2. Copilot に提案を頼む例:
   gh copilot suggest "このプロジェクトのREADMEを書いてください。内容は『GitHub Copilot CLIのデモプロジェクト』で、使い方も書いてください。"

  CI

   - .github/workflows/ci.yml に README の文法チェック（markdownlint）を行うワークフローを追加しています。

  貢献

  バグ報告や改善提案は Issue を作成してください。プルリク歓迎です。

  ライセンス

  自由に利用してください。
