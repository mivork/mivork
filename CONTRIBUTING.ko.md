# Contributing

*Languages: [English](CONTRIBUTING.md) · [日本語](CONTRIBUTING.ja.md) · [한국어](CONTRIBUTING.ko.md)*

이 저장소는 mivork의 프로필입니다. 공동 작업자를 환영합니다.

## Collaborators

- 공동 작업자는 GitHub의 **Settings → Collaborators**에서 초대합니다.
- 초대된 분은 Issue, PR, 커밋을 통해 변경을 제안할 수 있습니다.

## Commit rules

- 커밋 메시지는 [Conventional Commits](https://www.conventionalcommits.org/) 형식을 사용합니다 (예: `docs:`, `ci:`, `chore:`).
- AI의 도움으로 작성한 커밋에는 아래 Co-author 줄을 추가합니다.

  ```text
  Co-Authored-By: Claude Haiku 5.5 <noreply@anthropic.com>
  ```

- `main`에 직접 push하지 마시고, 브랜치를 만든 뒤 PR을 열어 주세요.

## Issues and PRs

- Issue나 PR을 열면, 종류와 언어에 맞춘 첫 답변이 자동으로 달립니다. 담당자가 나중에 응답합니다.
- 답변 내용이 부정확하다고 느끼시면 편하게 댓글을 남겨 주세요.

## Automation

| Workflow | 설명 |
| --- | --- |
| `ai-first-reply.yml` | Issue 또는 PR이 열리면 템플릿 첫 답변을 게시합니다 (API 불필요, 무료) |
| `daily-commit.yml` | 하루 5번 활동을 기록합니다 (JST 09:00, 14:00, 19:00, 00:00, 05:00) |

다음 저장소 Secret을 설정해 주세요.

- `GIT_AUTHOR_EMAIL`: 자동 커밋의 작성자 이메일 (GitHub 계정에 연결된 이메일이어야 합니다)

첫 답변은 항목의 종류와 언어를 판단해 템플릿을 반환하므로 API 키가 필요하지 않습니다.
