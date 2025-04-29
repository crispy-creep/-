# 늘벗튼튼 모션 인식 게임 (toy_project)

## 📌 프로젝트 개요

이 프로젝트는 **Mediapipe**를 활용하여 사용자의 모션을 실시간으로 인식하고, 이를 **게임 컨트롤러**로 활용하는 모션 인식 게임입니다. 몸의 움직임으로 캐릭터를 조작하거나 특정 동작을 수행하며 인터랙티브한 경험을 제공합니다.

## 📋 목차

1. [주요 기능](#주요-기능)
2. [설치 방법](#설치-방법)
3. [사용 방법](#사용-방법)
4. [프로젝트 구조](#프로젝트-구조)

## 🔥 주요 기능

- **실시간 모션 추적**: Mediapipe의 Hand, Pose 모듈을 사용하여 손 동작과 전신 움직임을 인식
- **게임 인터랙션**: 특정 포즈나 제스처를 통해 캐릭터를 이동, 점프, 공격 등 다양한 액션 수행
- **점수 시스템**: 게임 플레이 결과에 따라 실시간 점수 계산 및 표시
- **튜토리얼 모드**: 초보자도 쉽게 따라할 수 있는 가이드 모션 제공

## ⚙️ 설치 방법

```bash
# 1. 저장소 클론
git clone https://github.com/username/toy_project.git
cd toy_project

# 2. 가상 환경 생성 (추천)
python3 -m venv venv
source venv/bin/activate  # Windows: venv\\Scripts\\activate

# 3. 의존성 설치
pip install -r requirements.txt
```

## 🚀 사용 방법

1. 가상 환경 활성화
   ```bash
   source venv/bin/activate  # Windows: venv\\Scripts\\activate
   ```
2. `main.py` 실행
   ```bash
   python main.py
   ```
3. 화면에 나타나는 안내에 따라 카메라 위치를 조정하고, 모션 인식 범위 내에서 움직임을 수행하세요.
4. 게임 화면에서 캐릭터가 동작을 인식하여 반응합니다.

## 📁 프로젝트 구조

```
toy_project/
├── README.md         # 프로젝트 설명서
├── main.py           # 게임 실행 스크립트
├── game/             # 게임 로직 관련 모듈
│   ├── __init__.py
│   ├── controller.py # 모션 인식 컨트롤러
│   └── renderer.py   # 게임 화면 렌더링
└── utils/            # 유틸리티 함수 모음
    ├── mediapipe_utils.py
    └── score_utils.py
```
