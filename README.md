# Markdown-Usage
> 마크다운(MarkDown)사용법

# 1. 마크다운 사용법(문법)
## 1.1. 문서 제목
```
# This is the title1.
## This is the title2.
### This is the title3.
#### This is the title4.
##### This is the title5.
###### This is the title6.
```

# This is the title1.
## This is the title2.
### This is the title3.
#### This is the title4.
##### This is the title5.
###### This is the title6.
####### This is the title7.(1~6까지만 지원하고 7부터는 지원하지 않는다)

## 1.2. BlockQuote
블럭인용문자 ```>```를 사용한다.
```
> This is a first blockqute.
>	> This is a second blockqute.
>	>	> This is a third blockqute.
```
> This is a first blockqute.
>	> This is a second blockqute.
>	>	> This is a third blockqute.

`>`의 갯수에 따라 중첩 가능하다.
> 블럭 

> 다중 블럭1
>> 다중 블럭2
>> 다중 블럭3

다른 마크다운 요소를 포함할 수도 있다.\
(앞에서 사용한 회색칸을 만드는 방법은 아래 코드블럭 만드는 방식은 이용한다)

> ### This is the title3.
> * List
>	```
>	code
>	```

## 1.3. 목록
### ● 순서있는 목록(번호)
**순서있는 목록은 숫자와 점을 사용한다.
```
1. 첫번째
2. 두번째
3. 세번째
```
1. 첫번째
2. 두번째
3. 세번째

**모든 번호는 내림차순으로 정의된다.**
```
1. 첫번째
3. 세번째
2. 두번째
```
1. 첫번째
3. 세번째
2. 두번째

### ● 순서없는 목록(글머리 기호: `*`, `+`, `-` 지원)
```
* 빨강
  * 녹색
    * 파랑
```
(`*`, `+`, `-` 모두 사용 가능하며, 혼합해서 사용해도 상관없다)

## 1.4. 코드
4개의 공백 혹은 하나의 탭으로 들여쓰기를 사용하면 코드로 변환되기 시작하며, 들여쓰지 않은 행을 만날때까지 변환이 계속된다.(!! 이때 꼭 한 줄씩 띄어쓰기 해야 한다)

### 1.4.1. 들여쓰기
```
This is a normal paragraph:

    This is a code block.
    
end: This is not code block. 
```

실제 적용예:

***
This is a normal paragraph:

    This is a code block.

end: This is not code block.
***

> 한줄 띄어쓰지 않으면 문제가 발생한다.

```
This is a normal paragraph:
    This is a code block.
end: This is not code block.
```

실제 적용예:

***
This is a normal paragraph:
    This is a code block.
end: This is not code block.
***

### 2.4.1. 코드블럭
코드블럭은 다음과 같이 2가지 방식을 사용할 수 있:

* `<pre><code>{code}</code></pre>` 이용방식

```
<pre>
<code>
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }

}
</code>
</pre>
```

<pre>
<code>
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
</code>
</pre>

* 코드블럭코드("```") 을 이용하는 방법

<pre>
<code>
```
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
```
</code>
</pre>


```
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
```

* 문법 강조 기능: Syntax Highlighting은 코드블럭코드("```") 시작점에 사용하는 언어를 선언한다.

<pre>
<code>
```java
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
```
</code>
</pre>

```java
public class BootSpringBootApplication {
  public static void main(String[] args) {
    System.out.println("Hello, Honeymon");
  }
}
```


## 1.5. 수평선 ```<hr/>```
보통 페이지 나누기 용도로 사용하며,  3개 이상 사용해야 한다.

```
* * *

***

*****

- - -

---------------------------------------

**
```

* 적용예
* * *

***

*****

- - -

---------------------------------------

** 3개 미만은 수평선을 만들 수 없다.


## 1.6. 링크 연결

```
사용문법: [Title](link)
적용 예시: [Google](https://google.com, "google link")

이메일 링크: <address@example.com>
```
* Link: [Google](https://google.com, "google link")
* Email: <adress@example.com>

## 1.7. Highlight(`*`, `_` 사용)
```
*single asterisks*
_single underscores_
**double asterisks**
__double underscores__
~~cancelline~~
```

* *single asterisks*
* _single underscores_
* **double asterisks**
* __double underscores__
* ~~cancelline~~

## 1.8. 이미지 첨부
```
![Alt text](/path/to/img.jpg)
![Title](link)
```
![게임하는 곰돌이](https://img2.woyaogexing.com/2021/01/12/c553569abafe40a5aad5d1d42eb6daf7!400x400.webp)

사이즈 조절 기능은 없다.: ```<img width="" height=""></img>```를 이용

* 사용 예시:
```
<img src="/path/to/img.jpg" width="450px" height="300px" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>
<img src="/path/to/img.jpg" width="40%" height="30%" title="px(픽셀) 크기 설정" alt="RubberDuck"></img>
```

<img src="https://img2.woyaogexing.com/2021/01/12/c553569abafe40a5aad5d1d42eb6daf7!400x400.webp" width="450px" height="450px" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>
<img src="https://img2.woyaogexing.com/2021/01/12/c553569abafe40a5aad5d1d42eb6daf7!400x400.webp" width="40%" height="30%" title="%(비율) 크기 설정" alt="RubberDuck"></img>

## 1.9. 줄바꿈
`\` + `Enter`후 글을 작성하면 줄이 바뀐다. 
```
줄 바꿈을 하기 위해서는 문장 마지막에서 \를 사용하고 Enter 후 글을 작성해야한다.\
이렇게
```

줄 바꿈을 하기 위해서는 문장 마지막에서 \를 사용하고 Enter 후 글을 작성해야한다.\
이렇게

## 1.10. 테이블
* `|`을 기준으로 테이블이 구분되고, `-`으로 구분된 곳에 `:`으로 문자를 정렬할 수 있다.
* 첫번째 행은 `-`된다.

```
|테이블1|테이블2|테이블3|
|:---|:---:|---:|
|왼쪽정렬|중앙정렬|오른쪽정렬|
|여기서도|*강조 기능이*|**작동된다**|
```

|테이블1|테이블2|테이블3|
|:---|:---:|---:|
|왼쪽정렬|중앙정렬|오른쪽정렬|
|여기서도|*강조 기능이*|**작동된다**|

## 1.11. CheckList
* 체크리스트는 줄 앞에 `-[x]` 혹은 `-[ ]`써서 만들 수 있다.
* -[x] 이것은 완료된 항목이다. 
* -[ ] 이것은 완료되지 않은 항목이다. 

*****
# 2. 마크다운 꾸미기
## 2.1

***
## ○ 참고문헌
Markdown은 마크다운 사용법을 공부 목적으로 만들었으며, 아래 문서를 참고하였습니다.\
좀 더 자세한 설명을 원하시면 아래 문서를 참고해주세요.^^
* [John gruber 마크다운 번역](http://nolboo.github.io/blog/2013/09/07/john-gruber-markdown/)
* [깃허브 취향의 마크다운 번역](http://nolboo.github.io/blog/2014/03/25/github-flavored-markdown/)
* [[공통] 마크다운 markdown 작성법](https://gist.github.com/ihoneymon/652be052a0727ad59601)
* [GitHub Docs 기본 쓰기 및 서식 지정 구문](https://docs.github.com/ko/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
