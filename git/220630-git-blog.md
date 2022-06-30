# .gitignore, license and github blog

## .gitignore

> .gitignore 는 git이 파일을 추적할 때, 어떤 파일이나 폴더 등을 추적하지 않도록 명시하기 위해 작성하며, 해당 문서에 작성된 리스트는 수정사항이 발생해도 git이 무시하게 됨.

---

## license

> 오픈 소스에 대한 라이센스 정리

- MIT License
  - 모든 행동에 제약이 없고, 저작권자는 소프트웨어와 관련한 책임에서 자유로우므로 가장 많이 쓰임
- Apache License 2.0
  - 특허권 관련 내용이 포함됨
- GNU General Public License v3.0
  - 가장 많이 알려져있고, 의무사항이 존재함

---

## github blog

> github 저장소를 활용해 정적인 사이트 호스팅이 가능한데 이 때 `username`.github.io 레포지토리를 생성해 호스팅 가능하다. 레포지토리 생성 후에는 꼭 index.html 을 생성해주어야 한다.

> 밋밋한 블로그를 조금 더 블로그 스럽게 만들어주는 것들이 있는데 이를 static site generator 이라고 하며, Jekyll(Ruby), Hugo(Golang), Hexo(NodeJS) 등이 있다.

1. [Hexo 사이트 바로가기](https://hexo.io/ko/)
2. [Jekyll 사이트 바로가기](https://jekyllrb-ko.github.io/)
3. [Hugo 사이트 바로가기](https://gohugo.io/)

---

## Hexo 사용하기

> NodeJS 기반의 정적인 블로그 생성기로, 커스터마이즈가 쉬운 장점이 있다.

#### Hexo 설치

```
  $ npm install -g hexo-cli
```

#### 타켓 폴더의 Hexo 를 초기화

```
  $ hexo init <folder>
  $ cd <folder>
  $ npm install
```

#### 설치된 Hexo 설정파일인 \_config.yml 수정

##### 필수 수정 사항

- Site : blog 제목 및 작성자 등을 설정가능
- URL : 사용자의 github과 연결을 위해 url에 사용자 github 주소 기재
- Deployment : deploy 항목에 type, repo, branch 필수 입력

#### 새 포스트 만들기

```
  새 포스트 파일 만들기
$ hexo new post "포스트 이름"
  포스트 수정
$ 코드에디터 source/_posts/포스트 이름.md
  local에서 확인하기 위한 파일 재생성
$ hexo clean && hexo generate
  localhost:4000 에서 확인하기 위한 로컬서버 시작(종료할땐 ctrl+c)
$ hexo server
  문제없음을 확인한 후 repository에 업로드
$ hexo clean && hexo deploy
```

#### theme 설정

> Hexo 사이트 Themes 항목에서 원하는 테마 검색 후 설정방법 확인해 설정
