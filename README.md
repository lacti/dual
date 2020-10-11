# Dual

굉장한 에셋([game-icons.net](https://game-icons.net/))을 발견한 기념으로 만드는 웹 or 앱 1:1 게임

## 인증 및 로비

기존에 구현된 서버 사용

- [auth-api](https://github.com/yingyeothon/auth-api/)로 인증 토큰 획득
- [lobby-api](https://github.com/yingyeothon/lobby-api/)로 로비 접속

## 게임 서버

[dual](https://github.com/lacti/dual)

- AWS Lambda 기반의 게임 서버
  - 2명을 matching 받아서
  - 랜덤으로 card deck을 구성해서 분배
  - 각 턴마다 유저가 제출한 카드로 효과를 적용
  - 한 명의 HP가 모두 닳거나 혹은 모든 카드가 소진되면 게임 종료. 이 때 HP가 더 많이 남은 쪽이 승리

## 게임 클라이언트

앱 개발은 못 하기 때문에 간단히 Web으로 클라이언트를 구성할 예정.

## 게임 데이터

적당히 Google Spreadsheet로 효과 종류와 데미지 등을 작성하고 적당히 export해서 사용할 예정.

## License

MIT

