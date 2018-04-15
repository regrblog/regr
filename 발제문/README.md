## 발제문 작성법

발제문 디렉토리에는 다음과 같은 파일이 있습니다.

- `main.tex` : 마스터 문서 (이 문서를 컴파일한다)
- `elsarticle.cls` : 문서 클래스, [이곳](https://ko.sharelatex.com/templates/journals/elsevier)에서 다운로드 또는 [이곳](https://ctan.org/tex-archive/macros/latex/contrib/elsarticle)에서 설치 가능
- `regrstyle.sty` : 문총강을 위해 제작된 스타일시트
- `{언어 이름}/` : 각 발제문의 본문이 들어있는 언어별 디렉토리


이 중에서 `main.tex` 를 **XeLaTeX** 을 이용해 컴파일해야 하며, 이 때 다음과 같은 사항이 필요합니다.

- CMU Serif, CMU Sans Serif: [이곳](http://cm-unicode.sourceforge.net)에서 설치 가능
- KoPub 바탕, KoPub 돋움: [이곳](http://www.kopus.org/biz/electronic/font.aspx)에서 설치 가능


발제문 작성 시, 본문에 해당하는 `tex` 파일을 만들고, 적절한 디렉토리에 놓은 뒤, `main.tex` 를 열어, 아래 `\include` 함수의 인자에 상대 경로를 입력한 뒤, XeLaTeX 으로 컴파일합니다.

​```
\include{Chukchi/Chukchi_Minkyu_20180307}
​```

단, 파일 이름은 `{언어 이름}_YYYYMMDD_{발제자}.tex` 으로 통일하며, UTF-8 로 저장하는 것에 주의합시다.



작성이 끝나면, 작성한 `tex` 파일을 [구글 드라이브](https://goo.gl/23kaoy)에 업로드합니다.