# copilot-demo

GitHub Copilot CLIのデモプロジェクト

## 概要
このリポジトリは「GitHub Copilot CLIのデモプロジェクト」です。Copilot CLI（gh copilot）を使って提案を受けたり、READMEやコードの骨組みを生成する動作確認用に作成しました。

## 前提条件
- GitHub CLI（gh）がインストールされていること
- Copilot拡張が有効になっていること（gh extension install github/gh-copilot -- if needed）
- GitHubにログイン済みであること（`gh auth login`）

## 使い方
1. このディレクトリへ移動:
   ```powershell
   cd C:\Users\kikir\copilot-demo
   ```
2. CopilotにREADME作成を提案する例:
   ```powershell
   gh copilot suggest "このプロジェクトのREADMEを書いて。内容は『GitHub Copilot CLIのデモプロジェクト』で、使い方も書いて"
   ```
   - 提案を確認し、必要に応じて受け入れて編集してください。

## 追加作業
- READMEを受け入れたら、リポジトリをgitで初期化してコミットできます:
  ```powershell
  git init
  git add README.md
  git commit -m "Add README for copilot-demo"
  ```

## ライセンス
このデモは自由に使ってください。説明や手順の参考にどうぞ。
