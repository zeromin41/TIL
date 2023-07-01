## 블록구분

static void Main(string[] argo) { }

## 문법

### if문

if (부울식)
{
부울식이 참이면 실행할 코드블록
}
+
else if (부울식) 
{
부울식이 참이면 실행할 코드블록
}
+
else 
{
}

### for문

for (초기화; 조건; 반복자)                                                
// int=0, i<3, i++
{
조건이 true일때 실행할 코드블록
}

### while문

초기화;                                                                            

//int i = 0

while (부울식 or 조건식)                                
{
부울식이나 조건식이 true 일때 실행할 코드블록 
반복자(i++)
}

### break문

배치된 지점에서 가장 가까운 바깥쪽 루프를 종료

int i = 0;
while (i<10)

{
	if (i==1)
	{
		break;
	}		
 
실행할 코드블록;	
i++;

}

//i==0일때 if 문 실행안되어서 실행할 코드블록 실행됨. 
//i==1일때 if 문실행되고 break;문 실행되어서 가장 바깥쪽 루프종료. = while문 종료

### Foreach 문

배열이나 리스트를 순회하여 요소값에 접근함

int[] numbers = {1,3,5,7,9};

foreach(int num in numbers)
{
	Console.WriteLine(num);
}

### 딕셔너리

KeyValuePair<TKey,TValue>                     

//<키,값>

Dictionary<string, string> dic;                              

//dic 변수

dic = new Dictionary<string, string>();
dic.Add(“홍길동”, “01000000000”);
string hongNumber = dic[“홍길동”];
Console.WriteLine(hongNumber);  

//01000000000 출력

public TValue this[TKey key] {get; set;}    

//지정된 키에 연결된 값을 가져옴

변수.ContainsKey         

//키를 가지고 있는지

변수.Count         

// 요소 개수



