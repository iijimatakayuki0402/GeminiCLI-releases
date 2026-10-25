# GeminiCLI

Gemini API を使った Claude Code ライクなコーディング CLI（個人用）。コマンド名は `gcli`。

> **注意**: このリポジトリは配布物（インストーラー・npm パッケージ）のみを置く公開リポジトリです。ソースコードは公開していません。

---

## インストール

### Windows（PowerShell）

```powershell
irm https://github.com/iijimatakayuki0402/GeminiCLI-releases/releases/latest/download/install.ps1 | iex
```

### macOS / Linux

```sh
curl -fsSL https://github.com/iijimatakayuki0402/GeminiCLI-releases/releases/latest/download/install.sh | sh
```

### npm で直接インストール

```sh
npm install -g https://github.com/iijimatakayuki0402/GeminiCLI-releases/releases/latest/download/geminicli.tgz
```

---

## 動作要件

- **Node.js 22 以上**（[https://nodejs.org](https://nodejs.org)）

---

## はじめかた

### 1. 起動

```sh
gcli
```

### 2. API キーの設定

インタラクティブに設定する場合：

```sh
gcli login
```

環境変数で設定する場合：

```sh
export GEMINI_API_KEY="your-api-key"   # macOS / Linux
$env:GEMINI_API_KEY = "your-api-key"   # Windows PowerShell
```

> Gemini API キーは [Google AI Studio](https://aistudio.google.com/app/apikey) で取得できます。

---

## 更新

GeminiCLI は起動時（6時間ごと）に新しいバージョンを確認し、ヘッダーに通知します。

- `/update` コマンドまたは `gcli update` コマンドで即時更新
- 設定 `autoUpdate: true`（既定）で終了後に自動更新

---

## アンインストール

```sh
npm uninstall -g geminicli
```

---

## 操作ガイド

起動後に `/guide` と入力するとブラウザで操作ガイドが開きます。
