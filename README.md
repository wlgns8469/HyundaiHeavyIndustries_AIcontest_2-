# HyundaiHeavyIndustries_AIcontest_2-

##### Competition_No2 코드 실행 방법

## 0. 아나콘다 및 주피터 노트트북 실행
- Anaconda Prompt 실행
- 아래의 명령어 입력
	- conda activate yang
	- F:
	- jupyter notebook

## 1. 데이터셋 경로
- 폴더 구조는 과제 설명 자료와 같음
- dataset/test/ 에 01, 02, 03 폴더에 테스트 파일 위치

## 2.GTX.txt 파일 생성
##### 코드 실행 방법
- code/GTX_create.ipynb 실행
- run all
##### 실행과정 및 결과
- dataset/test 폴더의 01, 02, 03 폴더 내 GTX.txt파일 생성

## 3. 데이터 전처리
##### 코드 실행 방법
- code/Test_Data_Denoising.ipynb 파일 실행
- run all
##### 실행 과정 및 결과
- dataset/test/에 존재하는 테스트 파일에 대한 추론 전 데이터 전처리 과정
- denoising한 테스트 데이터셋은 dataset/test1 폴더에 저장

## 4. 테스트
##### 코드 실행 방법
- gt_test_01, gt_test_02, gt_test_03의 형식은 image_name.png\tGT\n 형식으로 저장되어 있어야한다. 이와같은 형식으로 되어있지 않을 경우 에러가 발생할 수 있음
- code/4.test.ipynb 파일 실행
- 두 번째 cell에 테스트할 파일 종류(01, 02, 03) 설정
- run all
##### 실행 과정 및 결과
- dataset/test1/'테스트할 파일 종류' 폴더에 있는 전처리된 테스트 파일에 대한 대한 추론 및 GT와 비교
- code 폴더 내 resault.csv파일 생성
