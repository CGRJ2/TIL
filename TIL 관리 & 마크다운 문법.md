
## **📌 TIL(Today I Learned) 작성 시 유용한 마크다운 문법 정리**

TIL(Today I Learned) 작성할 때 필요한 마크다운 문법을 정리해줄게!  
기본적인 문법부터 코드 블록, 테이블, 링크 등 중요한 요소들을 포함했어.

---

### **1. 제목(Heading)**

`#`을 사용해서 제목을 작성할 수 있어.  
`#`의 개수에 따라 제목의 크기가 달라짐.

```md
# 제목 1 (H1)
## 제목 2 (H2)
### 제목 3 (H3)
#### 제목 4 (H4)
##### 제목 5 (H5)
###### 제목 6 (H6)
```

📌 **결과**

# 제목 1

## 제목 2

### 제목 3

#### 제목 4

##### 제목 5

###### 제목 6

---

### **2. 글씨 스타일(굵기, 기울임, 취소선)**

```md
**굵은 글씨**
*기울임 글씨*
~~취소선~~
***굵은 기울임 글씨***
```

📌 **결과**  
**굵은 글씨**  
_기울임 글씨_  
~~취소선~~  
_**굵은 기울임 글씨**_

---

### **3. 리스트(목록)**

#### **✔ 순서 없는 목록 (Unordered List)**

```md
- 리스트 1
  - 하위 리스트 1
  - 하위 리스트 2
- 리스트 2
```

📌 **결과**

- 리스트 1
    - 하위 리스트 1
    - 하위 리스트 2
- 리스트 2

#### **✔ 순서 있는 목록 (Ordered List)**

```md
1. 첫 번째
2. 두 번째
3. 세 번째
```

📌 **결과**

1. 첫 번째
2. 두 번째
3. 세 번째

---

### **4. 코드 블록 (Code Block)**

#### **✔ 한 줄 코드 (Inline Code)**

```md
`Console.WriteLine("Hello, World!");`
```

📌 **결과**  
`Console.WriteLine("Hello, World!");`

#### **✔ 여러 줄 코드 블록 (Fenced Code Block)**

````md
```csharp
using System;

class Program
{
    static void Main()
    {
        Console.WriteLine("Hello, World!");
    }
}
````

````
📌 **결과**  
```csharp
using System;

class Program
{
    static void Main()
    {
        Console.WriteLine("Hello, World!");
    }
}
````

---

### **5. 링크 & 이미지**

#### **✔ 링크**

```md
[네이버](https://www.naver.com)
```

📌 **결과**  
[네이버](https://www.naver.com/)

#### **✔ 이미지**

```md
![대체 텍스트](https://via.placeholder.com/150)
```

📌 **결과**  
![대체 텍스트](https://via.placeholder.com/150)

---

### **6. 인용문 (Blockquote)**

```md
> 이 부분은 인용문입니다.
>> 중첩된 인용문
```

📌 **결과**

> 이 부분은 인용문입니다.
> 
> > 중첩된 인용문

---

### **7. 테이블 (Table)**

```md
| 제목1 | 제목2 | 제목3 |
|------|------|------|
| 값1  | 값2  | 값3  |
| 값4  | 값5  | 값6  |
```

📌 **결과**

|제목1|제목2|제목3|
|---|---|---|
|값1|값2|값3|
|값4|값5|값6|

---

### **8. 수평선 (Divider)**

```md
---
```

## 📌 **결과**

---

### **9. 체크리스트 (Task List)**

```md
- [x] 완료한 항목
- [ ] 미완료 항목
```

📌 **결과**

- [x]  완료한 항목
- [ ]  미완료 항목

---

### **10. 수식(LaTeX)**

옵시디언에서 수식을 사용하려면 `$`를 활용하면 돼.

```md
$E = mc^2$
```

📌 **결과**  
$E = mc^2$

---

### **🔹 TIL 예제 템플릿**

````md
# 📌 TIL - 2025.03.20

## 🔥 오늘 배운 내용
- 마크다운 문법 정리
- 옵시디언에서 코드 블록 사용법
- C# 문법 복습

## 📝 코드 예제
```csharp
using System;

class Program
{
    static void Main()
    {
        Console.WriteLine("Hello, Obsidian!");
    }
}
````

## 📌 참고 자료

- [옵시디언 공식 문서](https://help.obsidian.md/)
- [Markdown Guide](https://www.markdownguide.org/)



# 이모지 사용법 = `win` + `.`

