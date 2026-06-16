# copilot-demo

GitHub Copilot CLI のデモプロジェクト

## 概要
このリポジトリは GitHub Copilot CLI（gh copilot）の動作確認用デモプロジェクトです。Copilot CLI による提案受け取りや、README・コードの雛形生成を試すために作成しました。

## 前提条件
- GitHub CLI（gh）がインストールされていること
- Copilot 拡張が有効になっていること（必要なら `gh extension install github/gh-copilot`）
- GitHub にログインしていること（`gh auth login`）

## 使い方
1. プロジェクトディレクトリへ移動:
   ```powershell
   cd C:\Users\kikir\copilot-demo
   ```
2. Copilot に README 作成を提案する例:
   ```powershell
   gh copilot suggest "このプロジェクトのREADMEを書いて。内容は『GitHub Copilot CLIのデモプロジェクト』で、使い方も書いて"
   ```
3. 提案を保存する方法（例）:
   - クリップボードにコピーしてから上書き保存:
     ```powershell
     Get-Clipboard | Set-Content -Path .\README.md -Encoding UTF8 -Force
     ```
   - PowerShell のヒアストリングで直接書く:
     ```powershell
     @"
     （提案されたREADMEの本文をここに貼る）
     "@ | Set-Content -Path .\README.md -Encoding UTF8 -Force
     ```

## git にコミットする
既に git リポジトリでない場合:
```powershell
git init --initial-branch=main
git add README.md
git commit -m "Add README for copilot-demo"
```

## CI（簡単な説明）
- このリポジトリには README の文法チェックを行う GitHub Actions ワークフローを追加しています（.github/workflows/ci.yml）。

## ライセンス
このデモは自由に利用できます。手順や説明は参考としてご活用ください。
