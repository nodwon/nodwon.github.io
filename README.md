## Welcome to GitHub Pages

## (쉘 스크립트 관련) getopt 및 getopts 명령어
### getopt란?
**getopt 함수는 C인터페이스를 기반으로 POSIX 유틸리티 구문 지침을 따르는 명령**
### getopts란?
**명령 행 인수를 구문 분석하기 위한 내장 Unix 쉘 명령**
**command-line option을 분석하는데 사용**
---
## (리눅스 명령어 관련) sed 및 awk 명령어
### sed란?
**sed는 유닉스에서 텍스트를 분해하거나 변환하기 위한 프로그램이다**
#### 사용법

` sed 's/regexp/replacement/g' inputFileName > outputFileName`


#### 기타 sed 명령어
1. 치환 외에도 25개의 sed 명령을 사용하여 다른 형태의 단순한 처리가 가능하다. 이를테면, 다음의 경우 d 명령어를 사용하여 비어있거나 공백만 포함하는 줄을 삭제한다

`sed '/^ *$/d' inputFileName`


2. 필터로서의 사용 -유닉스에서 sed는 파이프 안에 필터로 종종 사용된다.

`generateData | sed 's/x/y/g'`


3.파일 기반 sed 스크립트 - 한 줄에 하나의 명령으로 여러 sed 명령을 subst.sed와 같은 스크립트 파일 안에 넣으면 유용할 수 있으며 -f 옵션을 사용하면 파일로부터 s/x/y/g와 같은 명령을 실행할 수 있다.

  `sed -f subst.sed inputFileName > outputFileName`
  
-----

### awk란?
**텍스트 형태로 되어있는 입력 데이터를 행과 단어 별로 처리해 출력하는것**
1. AWK는 문자열 데이터와 연관 배열(배열의 인덱스가 숫자가 아닌 임의의 값이 될 수 있는 배열), 정규 표현식을 주로 사용한다. AWK와 sed가 결합하면 간결하면서도 강력한 스크립팅이 가능하다.
+ 텍스트 파일의 전체 내용 출력.
+ 파일의 특정 필드만 출력.
+ 특정 필드에 문자열을 추가해서 출력.
+ 패턴이 포함된 레코드 출력.
+ 특정 필드에 연산 수행 결과 출력.
+ 필드 값 비교에 따라 레코드 출력.
![99C761465D1CBF9B28](https://user-images.githubusercontent.com/73088512/141676936-248c07f5-bb0a-43d4-8b04-176d22525341.png)
---
