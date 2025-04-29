name: 🐞 버그 리포트
description: 기능이 의도한 대로 작동하지 않을 경우
title: "[BUG] "
labels: [bug]
assignees:
  - ''
body:
  - type: markdown
    attributes:
      value: "버그 제보 감사합니다! 아래 내용을 최대한 자세히 작성해주세요."

  - type: input
    id: environment
    attributes:
      label: 사용 환경
      description: 운영체제, 브라우저, Node 버전 등
      placeholder: "예: Windows 11 / Chrome 123 / Node.js 20"
    validations:
      required: true

  - type: textarea
    id: steps
    attributes:
      label: 재현 단계
      description: 문제를 재현하는 순서를 단계별로 작성해주세요
      placeholder: |
        1. ...
        2. ...
        3. ...
    validations:
      required: true

  - type: textarea
    id: expected
    attributes:
      label: 기대 동작
      description: 기대했던 동작을 작성해주세요
    validations:
      required: true

  - type: textarea
    id: actual
    attributes:
      label: 실제 동작
      description: 실제 나타난 동작을 작성해주세요
    validations:
      required: true

  - type: textarea
    id: logs
    attributes:
      label: 콘솔 로그 / 오류 메시지
      description: 가능한 경우 로그를 붙여주세요 (예: 콘솔 출력, 스택 트레이스 등)
