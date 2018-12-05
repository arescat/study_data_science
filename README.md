# pulip_study_data_science

### 환경설정

1. 파이썬 설치(아나콘다)
* Visit : <https://www.anaconda.com/>
* Download
* Install
  * Select : Install for All Users
  * Folder : c:\Anaconda3

2. 환경변수(PATH) 추가
* \Anaconda3
* \Anaconda3\Scripts 
* \Anaconda3\Library\bin 

2-1. anaconda update
* conda update --all

3. 가상환경(virtual enviroment) 추가
* DOS(win) Prompt
  * conda create --name pstudy python=3.7
  * activate pstudy
  * deactivate
* Shell(Mac) Prompt
  * conda create --name pstudy python=3.7
  * source activate pstudy
  * source deactivate pstudy

4. 파이썬 설치 확인
  * python --version

5. 스터디 폴더
  * mkdir C:\Datascience\pstudy

6. jupyter notebook
  * cd C:\Datascience
  * jupyter notebook
