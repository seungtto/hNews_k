# hNews_k

[hNews](http://microformats.org/wiki/hnews)는 뉴스 콘텐츠용 마이크로포맷이다.
[hNews](http://microformats.org/wiki/hnews)는 [hAtom](http://microformats.org/wiki/hAtom)을 확장한 것으로 저널리즘과 관련된 과업을 보다 완전히 묘사할 수 있는 다수의 필드를 포함하고 있다.
[hNews_k](http://gemenon.snu.ac.kr:8888/wiki/Main_Page)는 [hNews](http://microformats.org/wiki/hnews)를 한국 상황에 맞게 가공한 것이다.
본 저장소에서는 [hNews_k](http://gemenon.snu.ac.kr:8888/wiki/Main_Page) 위키 소스코드와 XMDP(XHTML Meta Data Profiles)를 제공한다.


## 설치

[hNews_k](http://gemenon.snu.ac.kr:8888/wiki/Main_Page) 위키를 서버에 설치하기 위해서는 아래와 같은 기본 환경을 구축해야 한다.
 * Ubuntu 14.04+
 * PHP 5.5.9+
 * MySQL 5.0.2+

기본 환경을 구축한 다음, 이 저장소에서 [hNews_k](http://gemenon.snu.ac.kr:8888/wiki/Main_Page) 위키 소스코드를 다운로드한다.

```bash
$ cd /var/www/html
$ mkdir w
$ cd w
$ git clone https://github.com/seungtto/hNews_k.git
```

소스코드를 다운로드한 다음, 아래 URL에 접속하여 [미디어위키](https://www.mediawiki.org/)를 설치한다.
```bash
http://localhost(또는 서버 IP)/w/index.php
```
 * 언어 설정: 한국어
 * 저작권 및 이용 약관 확인
 * 데이터베이스 설정: MySQL
 * wiki 이름 및 관리자 계정 설정
 * 확장기능 설정: 모두 선택
 * LocalSettings.php 파일을 다운로드 받아 /var/www/html/w에 저장

설치를 마친 다음, LocalSettings.php 파일을 열어 [Dgraph](https://www.mediawiki.org/wiki/Skin:Dgraph)스킨 설정 라인을 추가한다.

```bash
$ cd /var/www/html/w
$ vi LocalSettings.php
```

```php
## add 2 lines
$wgDefaultSkin = "Dgraph";
wfLoadSkin( 'Dgraph' );
```


## 편집 및 이용

위키 이용에 관련된 참고 자료는 다음과 같다.
 * [위키 문법](https://ko.wikipedia.org/wiki/%EC%9C%84%ED%82%A4%EB%B0%B1%EA%B3%BC:%EC%9C%84%ED%82%A4_%EB%AC%B8%EB%B2%95)
 * [짧은 URL 적용](http://zetawiki.com/wiki/%EB%AF%B8%EB%94%94%EC%96%B4%EC%9C%84%ED%82%A4_%EA%B0%84%ED%8E%B8URL_%EC%A0%81%EC%9A%A9)
 * [위키 스킨 변경](https://www.mediawiki.org/wiki/Category:All_skins)

 
## 저작권

hNews_k 위키는 [MediaWiki](https://www.mediawiki.org/)와 [Dgraph Labs](https://dgraph.io/)의 저작권 정책을 따른다.
hNews_k 내 콘텐츠는 [hNews](http://microformats.org/wiki/hnews)의 저작권 정책을 따른다.
