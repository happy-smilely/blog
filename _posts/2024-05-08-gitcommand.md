---
title: "실무에서 사용하는 Git 명령어 총정리"
date: 2024-05-08 00:00:00 +09:00
categories: [Git, Version Control]
tags:
  [
    Git,
    Version Control,
    Development
  ]
---

> 실무에서 자주 사용하는 Git 명령어를 정리한 기록
{: .prompt-tip }

 Git은 분산 버전 관리 시스템으로, 소프트웨어 개발에서 코드의 버전을 관리하고 협업을 도와줍니다. 이 포스팅에서는 실무에서 자주 사용하는 Git 명령어를 정리합니다.

## Git 기본 명령어

 Git을 처음 사용할 때 필요한 기본 명령어들입니다.

### 저장소 초기화

 새로운 Git 저장소를 초기화하거나 기존 저장소를 클론할 수 있습니다.

```sh
git init  # 새로운 Git 저장소 초기화
git clone <repository_url>  # 기존 저장소 클론
```

### 변경 사항 추적

 작업 디렉토리의 변경 사항을 추적하고, 스테이지에 추가하며, 커밋합니다.

```sh
git status  # 현재 작업 디렉토리의 상태 확인
git add <file>  # 특정 파일을 스테이지에 추가
git add .  # 모든 변경 사항을 스테이지에 추가
git commit -m "커밋 메시지"  # 변경 사항을 커밋
```

## 브랜치 관리

 브랜치를 생성하고, 변경하며, 병합하는 방법입니다.

```sh
git branch  # 로컬 브랜치 목록 확인
git branch <branch_name>  # 새로운 브랜치 생성
git checkout <branch_name>  # 특정 브랜치로 이동
git checkout -b <branch_name>  # 브랜치를 생성하고 이동
git merge <branch_name>  # 브랜치를 현재 브랜치에 병합
git branch -d <branch_name>  # 로컬 브랜치 삭제
```

## 원격 저장소 관리

 원격 저장소와 로컬 저장소를 동기화하는 방법입니다.

```sh
git remote -v  # 원격 저장소 목록 확인
git remote add <name> <url>  # 새로운 원격 저장소 추가
git fetch <remote>  # 원격 저장소의 변경 사항 가져오기
git pull <remote> <branch>  # 원격 브랜치의 변경 사항을 로컬로 가져와 병합
git push <remote> <branch>  # 로컬 브랜치의 변경 사항을 원격 저장소로 푸시
```

## 파일 및 변경 이력 확인

 파일의 변경 이력을 확인하고, 변경 내용을 비교하는 방법입니다.

```sh
git log  # 커밋 로그 확인
git log --oneline  # 간단한 커밋 로그 확인
git show <commit>  # 특정 커밋의 상세 정보 확인
git diff  # 작업 디렉토리와 스테이지의 변경 내용 비교
git diff <source_branch> <target_branch>  # 두 브랜치 간의 변경 내용 비교
```

## 기타 유용한 명령어

 실무에서 유용하게 사용할 수 있는 기타 명령어들입니다.

```sh
git stash  # 현재 작업 내용을 임시로 저장
git stash pop  # 임시로 저장한 내용 복원
git rebase <branch>  # 현재 브랜치를 특정 브랜치의 최신 커밋으로 재배치
git cherry-pick <commit>  # 특정 커밋을 현재 브랜치에 적용
git tag <tag_name>  # 태그 생성
git tag -d <tag_name>  # 태그 삭제
git blame <file>  # 파일의 각 라인에 누가 마지막으로 변경했는지 확인
```

이러한 Git 명령어들을 숙지하고 사용하면, 실무에서의 코드 관리와 협업이 훨씬 효율적으로 이루어질 수 있습니다.
