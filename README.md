# ModuëAtlas 🗺️

**ModuëAtlas**는 방대한 로봇 학습 데이터셋의 구조와 내용을 깊이 있게 들여다보고 분석할 수 있는 데이터 익스플로러 패키지

---

## ✨ What is "Moduë"? (Etymology)

* **Origin**: 한국어 **"모두의" (Modu-ui)**에서 유래되었으며, "모두를 위한(Everyone's)"이라는 의미를 담음
* **Pronunciation**: **"Modue or Moduë" (모두에 /mo.du.e/)**로 발음하며, 포용성과 개방성을 상징
* **Vision**: 복잡한 로봇 데이터를 연구자 **모두가** 쉽고 명확하게 이해할 수 있도록 데이터의 지도를 제공

> **ModuëAtlas** = **Moduë** (Everyone's) + **Atlas** (A map for complex datasets)

---

## 🔍 Key Features

- **Unified Dataset Viewer**: **OXE(Open X-Embodiment)**, **LeRobot**, **Droid** 등 서로 다른 포맷의 데이터를 통합된 인터페이스로 확인
- **Trajectory Inspection**: 로봇의 궤적(Trajectory)과 액션(Action) 데이터를 시계열로 시각화
- **Statistic Analytics**: 데이터셋의 분포, 성공률, 센서 데이터의 이상치(Outlier) 등을 통계적으로 분석
- **Format Converter**: 다양한 로봇 데이터를 학습 프레임워크에 맞는 포맷으로 손쉽게 변환 및 필터링

---

## 🛠️ Usage

```python
import modueatlas

# 로봇 데이터셋 로드 (예: LeRobot)
dataset = modueatlas.load("lerobot/pusht")

# 데이터셋의 통계 및 궤적 요약 확인
modueatlas.summarize(dataset)

# 대화형 뷰어 실행
modueatlas.launch_viewer(dataset)
