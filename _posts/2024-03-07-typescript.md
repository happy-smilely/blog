---
title: "[Language] TypeScript 기록"
date: 2024-03-07 00:00:00 +09:00
categories: [Language, TypeScript]
tags:
  [
    language,
    typeScript,
    study
  ]
---

> React, Node.js (express) 구축하면서 공부했던 TypeScript 에 대한 기록 
{: .prompt-tip }

TypeScript은 JavaScript의 확장이자, 정적 타입 체크를 제공하는 프로그래밍 언어입니다. JavaScript로 컴파일되며, 큰 프로젝트를 관리하고 유지보수하기 쉽도록 도와줍니다.

## 주요 특징

- **정적 타입 지원**: TypeScript는 변수, 매개변수, 함수 등에 타입을 명시할 수 있어서 코드를 보다 안정적으로 만들어줍니다.

- **클래스와 모듈 지원**: JavaScript의 클래스와 모듈 시스템을 보완하여 객체지향 프로그래밍을 더 쉽게 할 수 있습니다.

- **ES6+ 기능 지원**: 최신 ECMAScript 표준 기능을 사용할 수 있으며, TypeScript는 이러한 기능을 편리하게 사용할 수 있도록 지원합니다.

- **강력한 개발 도구**: TypeScript는 코드 어시스트, 정적 분석 등을 통해 개발자에게 풍부한 개발 경험을 제공합니다.

- **타입 추론**: 타입을 명시하지 않아도 TypeScript가 자동으로 타입을 추론하여 오류를 줄여줍니다.

## 장점

- **타입 안정성**: 정적 타입 체크로 인해 런타임 에러를 줄여줍니다.

- **유지보수 용이성**: 명시적인 타입 정의와 모듈화로 코드의 가독성을 높이고 유지보수를 쉽게 만들어줍니다.

- **성능 향상**: 빠른 개발과 실행 속도를 제공하여 프로덕션 환경에서의 성능을 향상시킵니다.

## 사용 예시
```typescript
// 숫자를 더하는 함수
function addNumbers(num1: number, num2: number): number {
    return num1 + num2;
}

// 숫자 변수들
let firstNumber: number = 10;
let secondNumber: number = 20;

// 함수 호출과 결과 출력
let result: number = addNumbers(firstNumber, secondNumber);
console.log("덧셈 결과:", result);
```
## 분야

- **웹 개발**: Angular, React, Vue.js 등의 프레임워크에서 TypeScript를 기본 언어로 사용합니다.

- **Node.js 개발**: Express.js 등의 백엔드 프레임워크에서도 TypeScript를 사용하여 서버를 개발할 수 있습니다.

- **데이터 시각화**: D3.js와 함께 TypeScript를 사용하여 데이터 시각화 애플리케이션을 개발할 수 있습니다.

- **게임 개발**: Phaser.js 등의 게임 엔진에서 TypeScript를 사용하여 게임을 개발할 수 있습니다.
