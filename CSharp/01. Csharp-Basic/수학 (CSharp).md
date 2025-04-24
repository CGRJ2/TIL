
최대공약수와 최소공배수

```csharp
static int GCD(int a, int b)     //최대공약수 (유클리드 호제법)
    {
        while (b != 0)
        {
            int temp = b;
            b = a % b;
            a = temp;
        }
        return a;
    }

static int LCM(int a, int b)     //최소공배수
{
    return a * b / GCD(a, b);
}
```

****유클리드 호제법***
즉, 어떤 수 `a`를 `b`로 나누면,  
몫 `q`, 나머지 `r`가 생기고 그 관계는 이렇게 됨.
```
a = b × q + r     (단, 0 ≤ r < b)
```
`d`는 `a`,`b`의 공약수라고 하자.

이는 `a = bq + r` 에서  `d`로 나눈다면

`a`와 `b` 둘 모두 d로 나눠지니까 `a`와 `bq` 는 `d`로 나누어 떨어질 것이다.
그렇다는 것은 `r`또한 `d` 로 나누어 떨어질 것이라는 뜻이다.
그러므로 `a`와 `b`의 공약수는 `b`와 `a % b`(나머지)의 공약수와 같다.
이를 반복해서 나머지가 0이 될때의 값이 최대공약수가 된다.



소수(Prime Number) 판별
- 1과 자기 자신만 나누어 떨어지는 수

```csharp
// 이해를 돕기 위한 버전
static bool isPrime(int n)
{
	int divCount = 0;
	
	for (int i = 1;, i <= numb; i++)
	{
		if (n % i == 0) divCount += 1;
	}
	
	if (divCount == 2) return true;
	else return false;
}

// 최적화 버전 *실전용*
static bool isPrime(int n)
{
    if (n < 2) return false;

    for (int i = 2; i * i <= n; i++)
    {
        if (n % i == 0)
            return false;
    }
    return true;
}

```

시프트 연산?
