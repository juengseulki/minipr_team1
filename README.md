# 📒 1 Team Mini Project 회고록

<p align="center">

![GitHub repo size](https://img.shields.io/github/repo-size/juengseulki/minipr_team1)
![GitHub last commit](https://img.shields.io/github/last-commit/juengseulki/minipr_team1)
![GitHub contributors](https://img.shields.io/github/contributors/juengseulki/minipr_team1)
![GitHub stars](https://img.shields.io/github/stars/juengseulki/minipr_team1?style=social)

</p>

> 1팀 미니 프로젝트 진행 과정에서 겪었던 문제와 해결 과정, 그리고 협업 경험을 정리한 회고록입니다.

---

## 📑 목차

- [🚨 1. Git 충돌 에러](#-1-git-충돌-에러-conflict-error)
  - [📌 1-1. push 오류 발생](#-1-1-push-오류-발생)
  - [🔧 1-2. 해결 방법](#-1-2-해결-방법)
  - [⚠ 1-3. 같은 파일 충돌](#-1-3-같은-파일-같은-위치-수정-시-발생하는-충돌)
- [✏ 2. 오타 (Typo)](#-2-오타-typo)
- [💬 1팀의 협업 방식 개선](#-1팀의-협업-방식-개선)
- [📝 느낀 점](#-미니-프로젝트를-하면서-느낀-점)
- [🎯 프로젝트를 통해 배운 점](#-프로젝트를-통해-배운-점)

---

## 🚨 1. Git 충돌 에러 (Conflict Error)

### 📌 1-1. push 오류 발생

![push 오류](/image/image.png)

에러 메시지 핵심:

```bash
error: failed to push some refs to
```

### ✔ 원인

- 원격 저장소가 로컬보다 최신 상태일 때
- 팀원이 먼저 push를 진행했을 때

👉 원격 저장소에 내가 가지고 있지 않은 변경 사항이 존재할 경우 발생합니다.

---

### 🔧 1-2. 해결 방법

#### ✔ Step 1. pull

```bash
git pull origin
```

![pull 과정](/image/image-2.png)

#### ✔ Step 2. push

```bash
git push origin
```

![push 성공](/image/image-3.png)

#### 📌 기본 작업 순서

```text
add → commit → pull → push
```

---

### ⚠ 1-3. 같은 파일, 같은 위치 수정 시 발생하는 충돌

![충돌 에러](/image/image-4.png)

```bash
<<<<<<< HEAD
내 코드
=======
팀원 코드
>>>>>>> branch-name
```

![충돌 표시 화면](/image/image-5.png)

#### 🛠 해결 방법

1. 구분자 삭제
2. 최종 코드만 남김

```bash
git add .
git commit -m "conflict 해결"
git push origin
```

📌 대부분 소통 부족에서 발생 → 회의 후 수정하는 것이 바람직합니다.

---

## 💬 1팀의 협업 방식 개선

- ✅ push 후 디스코드 공유
- ✅ 작업 전 pull 먼저 진행
- ✅ 충돌 발생 시 즉시 팀원과 논의

---

## ✏ 2. 오타 (Typo)

![오타 예시](/image/image-6.png)

코딩 중 사소한 오타 하나로도:

- 코드가 실행되지 않거나
- 오류가 발생할 수 있습니다.

### ✔ 예방 방법

- 코드 천천히 다시 읽기
- 팀원 코드 리뷰
- push 전 명령어 재확인

> 작은 실수도 협업에서는 큰 영향을 줄 수 있음을 배웠습니다.

---

## 📝 미니 프로젝트를 하면서 느낀 점

|    이름     |                                                                                                                                                            느낀 점                                                                                                                                                            |
| :---------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
| **정슬기**  | 이번 미니 프로젝트를 통해 내가 알고 있는 부분을 팀원들에게 설명하며 복습할 수 있어 유익했다. Git 기능을 직접 활용하며 협업을 경험했고, 팀장의 역할에 대해 다시 생각해보는 계기가 되었다. 페이지 제작 전 구조를 설계하고 계획에 따라 코딩하면서 체계적인 작업 방식의 중요성을 배웠다. 협업 속에서 소통의 중요성을 깊이 느꼈다. |
| **강정민**  |                                                                                                                                                                                                                                                                                                                               |
| **김상우A** |                                                                                                                                                                                                                                                                                                                               |
| **신영미**  |                                                                                                                                                                                                                                                                                                                               |
| **심현수**  |                                                                                                                                                                                                                                                                                                                               |
| **이진한**  |                                                                                                                                                                                                                                                                                                                               |
| **정다희**  |                                                                                                                                                                                                                                                                                                                               |

---

## 🎯 프로젝트를 통해 배운 점

- 협업에서는 **소통이 가장 중요하다**
- push 전 반드시 **pull을 확인하는 습관**
- 작은 오타도 큰 오류로 이어질 수 있다
- 계획 후 코딩이 작업 효율을 높인다

---

<p align="center">
  ⭐ Team 1 Mini Project Reflection ⭐
</p>
