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

- Issue や PR を開くと、内容に応じた一次返信が自動で付きます。これは AI が生成したもので、担当者が後ほど確認します。
- 返信内容が不正確な場合は、遠慮なくコメントしてください。

## Automation

| Workflow | 内容 |
| --- | --- |
| `ai-first-reply.yml` | Issue / PR 作成時に GitHub Models で一次返信を投稿 |
| `daily-commit.yml` | 1日5回（JST 09:00 / 14:00 / 19:00 / 00:00 / 05:00）にアクティビティを記録 |

リポジトリの Secrets に以下を設定してください。

- `GIT_AUTHOR_EMAIL` … 自動コミットの作成者メール（GitHub アカウントに紐づくもの）

一次返信は GitHub Models の無料枠を使い、API キーは不要です（レート制限あり）。
任意の Variable `AI_MODEL` を設定するとモデルを変更できます（未設定時は `openai/gpt-4o-mini`）。
