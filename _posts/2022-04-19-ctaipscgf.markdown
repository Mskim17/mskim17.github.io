---
layout: post
title:  주차유도 셋팅 메뉴얼 v1.2
date:   2022-04-19 15:01:35 +0300
image:  ctaipscgf.jpg
tags:   Resources
---
6면/12면 카메라 메뉴얼

## 1. 차번 영역 프로그램 실행 방법

![]({{ site.baseurl }}/images/ctaipscgf/11.jpg)

1. 해당 프로그램을 실행 한다.
2. 12면 카메라 세팅은 위쪽 체크박스 클릭
3. 6면 카메라 세팅은 아래쪽 체크박스 클릭

### 2. 차번 영역 프로그램 실행방법 (12면)

![]({{ site.baseurl }}/images/ctaipscgf/12.jpg)

![]({{ site.baseurl }}/images/ctaipscgf/13.jpg)

* 이미지 가져오기 버튼 클릭 후, 다음 그림같이 영역 세팅
* 1~12번까지의 숫자는 아이콘 배치에 따라 순서가 달라질수도 있음.

![]({{ site.baseurl }}/images/ctaipscgf/14.jpg)

![]({{ site.baseurl }}/images/ctaipscgf/15.jpg)

* 정보 저장 클릭 후 저장 파일은 프로그램 안의 'data' 폴더안에 저장 됨.

![]({{ site.baseurl }}/images/ctaipscgf/16.jpg)

* 설정 파일 선택의 '...' 클릭하면 'data'폴더가 자동으로 열림
* 수정 할 파일을 더블클릭 하면 해당 파일의 주차영역 파일이 나옴 수정 후 다시 '정보저장' 클릭

### 3. 프로그램 올리는 법 (12면/6면 시스템 동일)

![]({{ site.baseurl }}/images/ctaipscgf/17.jpg)

* 영상 분석기 1번부터 순서대로 101 ~ N번 까지 적용
* 12면 주차유도 시스템은 192.168.40.101 ~ 192.168.40.N 까지 적용 (위 사진으로 봤을 경우 192.168.40.111까지 적용) 
* 6면 주차유도 시스템은 192.168.101.101 ~ 192.168.101.N 까지 적용 (위 사진으로 봤을 경우 192.168.101.111까지 적용) 

![]({{ site.baseurl }}/images/ctaipscgf/18.jpg)

* Chomre, explore창으로 192.168.40.101 접속하여 'Choose File' 선택
* 파일 선택 후 파일 업로드 설정하면 완료
* 12면 주차유도는 최대 24개까지 / 6면 주차인식은 최대 64개까지 업로드 가능

### 4. Device Manager 사용법 (카메라 IP를 찾는 프로그램)

![]({{ site.baseurl }}/images/ctaipscgf/19.jpg)

![]({{ site.baseurl }}/images/ctaipscgf/20.jpg)

* IP Search 클릭 후 통신 정상 네트워크는 그림과 같이 순차적으로 발생
- 20.1번이 도면상에서 1번 카메라

### 5. 프로그램 기초 데이터 세팅 방법 (12면)

![]({{ site.baseurl }}/images/ctaipscgf/21.jpg)

![]({{ site.baseurl }}/images/ctaipscgf/22.jpg)

* CPLSViewer 폴더 안에 들어가 LPSManagerNew 프로그램 실행
* 프로그램 실행 후 '초기 세팅' 버튼 클릭

![]({{ site.baseurl }}/images/ctaipscgf/23.jpg)

* '파일열기' 클릭 후 엑셀 기초 자료 만들어 두었던 파일 클릭 후 저장 버튼 누르면 완료.
- 단, 저장 버튼 누르고 '완료 되었습니다.' 라는 팝업 창이 나올 때까지 종료 금지 (도중 닫아버리면 데이터 생성이 모두 안됨)
* 생성 후, Query Browser 들어가서 dev_info에서 엑셀 기초 자료 개수 만큼 Dev_id 생성되면 성공적으로 완료

![]({{ site.baseurl }}/images/ctaipscgf/24.jpg)

* CPLSViewer 폴더 안의 CPLSViewer-아이콘 프로그램 실행
* Query Browser 테이블 중 2개의 테이블 확인 (ID: lpsadmin / PW: lpsadmin)
- Dev_Icon_Floor = 카메라 아이콘 배치 테이블
- Park_Icon_Floor = 주차 아이콘 배치 테이블