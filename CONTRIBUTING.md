# Contributing

このリポジトリは mivork のプロフィールです。共同開発者を歓迎します。

## Collaborators

- 共同開発者は GitHub の **Settings → Collaborators** から招待されます。
- 招待された人は、Issue・PR・コミットを通じて変更を提案できます。

## Commit rules

- コミットメッセージは [Conventional Commits](https://www.conventionalcommits.org/) 形式（例: `docs:`, `ci:`, `chore:`）にします。
- AI 支援で書いたコミットには、以下の Co-author 行を付けます。

  ```text
  Co-Authored-By: Claude Haiku 5.5 <noreply@anthropic.com>
  ```

- `main` へ直接 push せず、ブランチを切って PR を出してください。

## Issue / PR

- Issue や PR を開くと、種類（バグ報告・質問・PR など）と言語に応じた一次返信が自動で付きます。担当者が後ほど対応します。
- 返信内容が不正確な場合は、遠慮なくコメントしてください。

## Automation

| Workflow | 内容 |
| --- | --- |
| `ai-first-reply.yml` | Issue / PR 作成時に定型文で一次返信を投稿（API 不要・無料） |
| `daily-commit.yml` | 1日5回（JST 09:00 / 14:00 / 19:00 / 00:00 / 05:00）にアクティビティを記録 |

リポジトリの Secrets に以下を設定してください。

- `GIT_AUTHOR_EMAIL` … 自動コミットの作成者メール（GitHub アカウントに紐づくもの）

一次返信は Issue / PR の種類と言語を判定して定型文を返すため、API キーは不要です。
