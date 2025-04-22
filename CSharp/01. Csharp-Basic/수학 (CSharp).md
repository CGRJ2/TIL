
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
