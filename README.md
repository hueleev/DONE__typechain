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

## 3. Types in Typescript

```ts
const sayHi = (name:string, age:number, gender:string): string => { // param/return type 지정 가능
    return `Hello ${name}, you are ${age}, you are a ${gender}`;
};

console.log(sayHi("Nicolas", 44, "male"));
```

* `tsc-watch` 추가 (ts코드가 수정될 때마다 자동으로 컴파일)

* `tsconfig.json` 설정 수정 (`dist`에 컴파일된 파일 저장하도록 변경)