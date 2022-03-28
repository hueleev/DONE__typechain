#  Typescript로 블록체인 만들기

**TypeScript** 👍 super set of JavaScript

---

## 1. Setting Typescript up

```
npm install typescript
```

명령어 ```tsc``` 컴파일 시작

index.ts -> index.js/index.js.map 생성

---

## 2. First steps with Typescript

```ts
const name = "Nicolas",
    age = 24,
    gender = "male";

const sayHi = (name, age, gender) => { // gender뒤에 ? 붙이면 선택적param!
    console.log(`Hello ${name}, you are ${age}, you are a ${gender}`)
}

sayHi(name, age); // param이 2개이므로 컴파일 실패

export {};
```
