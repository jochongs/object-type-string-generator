# Object Type 문자열 생성기
* Object 데이터 값의 타입을 확인하여 key: type 형태의 JSON string을 만들어주는 함수

```javascript
// 예시
generateTypeObject({
    name: 'jochong',
    age: 22,
    tests: [{
        name: 'test1',
        description: 'description1',
        numbers: [1, 2, 3]
    }]
});

// 결과
{
    "name": string,
    "age": number,
    "tests": {
        "name": string,
        "description": string,
        "numbers": number[],
    }[],
}
```