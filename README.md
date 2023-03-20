# Colab과 Github 연동
----

##### Colab에서 따로 빼둔 commit 파일 코드 창에서 실행

### 1. Google Drive 접근

```
from google.colab import drive
drive.mount('/content/drive')
```

### 2. Commit을 원하는 폴더로 이동
```
cd /content/drive/MyDrive/Commit_to_github/Colab-DL
```

### 3. 본인임을 확인
```
!git config --global user.email '(user email)'
!git config --global user.name '(user name)'
```

### 4. 폴더 add (폴더 아래 전체에 대해서, 만약 파일 하나만 하고 싶으면 파일명까지 적기)
```
!git add .
```

### 5. commit 하기
```
!git commit -m '원하는 아무 메시지'
!git push # push할 때 브랜치 확인!
```
