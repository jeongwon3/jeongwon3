<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&amp;color=0:0F172A,55:1D4ED8,100:0891B2&amp;height=190&amp;text=Jeongwon%20Park&amp;desc=Autonomous%20Driving%20Perception&amp;fontColor=FFFFFF&amp;fontSize=46&amp;fontAlignY=33&amp;descAlignY=55&amp;descSize=17" alt="Jeongwon Park · Autonomous Driving Perception" />
</div>

# 박정원 · Jeongwon Park

**Autonomous Driving Perception · 3D Occupancy · Embedded AI**

## 👋 About Me

가천대학교 인공지능학과에서 공부하며, 자율주행 차량과 로봇이 주변 환경을 인식하는 시스템을 개발하고 있습니다.

ROS에서 카메라 검출 결과와 LiDAR 클러스터를 정합하는 모듈을 구현했습니다. 로보티즈 Perception 팀에서는 보행자 신호등 검출 성능 개선을 위해 학습 데이터 구성과 모델을 비교하고, Jetson Orin에서 검출 정확도와 추론 속도를 측정하는 벤치마크를 개발했습니다.

최근에는 CARLA의 다중 카메라 영상으로 3D Occupancy를 예측하는 모델을 학습하고, 시뮬레이터의 지도와 차량 메시를 활용해 프레임별 Occupancy GT를 생성하고 있습니다.

## 🔍 Research Interests

- **3D Perception** · Camera-only 3D Occupancy, BEV, 깊이 추정
- **Sensor Fusion** · LiDAR–Camera 좌표 정합, 투영, 객체 매칭
- **SLAM & Localization** · LiDAR SLAM, 협업 SLAM, 맵 정합
- **Embedded AI** · Jetson 기반 모델 추론과 성능 분석

## 🛠️ Tech Stack

| 분야 | 기술 |
| --- | --- |
| Programming | Python, C, C++ |
| Deep Learning & Vision | PyTorch, MMDetection, YOLO/YOLOX, DETR/RT-DETR |
| Robotics & Simulation | ROS 1, ROS 2, CARLA, Cartographer |
| Edge Inference | NVIDIA Jetson Orin, TensorRT, ONNX Runtime, CUDA |
| Development | Ubuntu, Docker, Git |

## 💼 Experience

| 소속 | 역할 | 주요 활동 |
| --- | --- | --- |
| **ROBOTIS Perception Team** | Perception Intern · 2026 | 보행자 신호등 검출 모델 학습·평가, Jetson Orin 추론 벤치마크, CARLA 기반 3D Occupancy 실험 |
| **GADIS** | 인지팀원 · 2025 / 인지팀 리더 · 2026 | 자율주행 인지 모듈 개발 및 경진대회 참여 |
| **Vehicle Intelligence Perception Lab** | 학부연구생 | 모빌리티 인지 연구, 컴퓨터 비전 논문 세미나, 협업 SLAM 프로젝트 |
| **Autonomous Mobility Systems Lab** | 학부연구생 | 자율주행 인지 관련 연구 활동 |
| **SCUD Formula Student Racing Team** | 엔지니어링 팀원 · 2025 | Formula Student 팀 활동 및 KSAE E-Formula 경진대회 참여 |

## 🚀 Projects

| 프로젝트 | Description | 기술 |
| --- | --- | --- |
| **[FlashOCC for CARLA](https://github.com/jeongwon3/FlashOcc)** | 4대 카메라 영상으로 3D 의미 점유를 예측하도록 FlashOCC를 CARLA에 적용했습니다. 깊이 보조 손실과 클래스 가중치를 비교하고, 광선의 첫 점유 위치를 분석해 실제 물체 앞에 나타나는 오검출을 확인했습니다. | PyTorch, FlashOCC, CARLA |
| **CARLA Asset-based Occupancy GT** | CARLA 지도 4종과 차량 메시 23종을 확보했습니다. 녹화 프레임의 차량 ID와 자세로 차량을 배치하고, 지도와 차량을 자차 좌표계에 정렬한 뒤 메시 표면을 복셀화했습니다. 센서 시야에서 가려진 곳도 에셋이 배치된 영역의 점유 표면을 생성할 수 있습니다. | CARLA 0.9.16, GLB/glTF, Python, C++ |
| **보행자 신호등 검출 성능 개선** | 보행자 신호등 검출 성능을 높이기 위해 학습 데이터 구성과 검출 모델을 비교·평가했습니다. Jetson Orin에서 모델별 검출 정확도(mAP·Precision·Recall)와 추론 성능(FPS·P99 지연 시간)을 동일한 조건으로 측정하는 벤치마크를 개발했습니다. | YOLOX, MMDetection, Jetson Orin, TensorRT, ONNX Runtime |
| **LiDAR–Camera Fusion Object Selection** | YOLO 검출 박스와 LiDAR 클러스터를 연결하는 좌표 변환·투영·매칭 로직을 설계했습니다. 거리 필터링을 적용하고 독립 ROS 노드로 통합했습니다. | ROS, YOLO, LiDAR |
| **Collaborative SLAM Map Merging** | LIMO 로봇과 Cartographer로 실내 구역별 2D 점유 지도를 생성했습니다. 지도 간 특징점을 매칭해 회전과 이동을 추정하고, 로컬 맵을 하나의 전역 지도로 병합했습니다. | LIMO, Cartographer, ROS |

## 🏆 Contests & Awards

| 연도 | 대회 | 결과 |
| --- | --- | --- |
| 2026 | 국제 대학생 e-Mobility Expo EV 자율주행 경진대회 | **1차 1위** |
| 2025 | 해양 KMOU AI 모빌리티 글로벌 대회 | **자율주행 레이싱 대상** · 디지털 트윈 장려상 |
| 2025 | 대학생 창작모빌리티 경진대회 | **장려상** |
| 2025 | KSAE E-Formula 경진대회 | **4위** |

## 🎓 Education & Activities

- **가천대학교 인공지능학과** · 2027년 2월 졸업 예정 · 스마트카 마이크로디그리 이수
- **현대자동차·현대엔지비 H-모빌리티 클래스** · 자율주행 인지 트랙, 2026
- **가천대학교 Physical AI Research Camp** · Jetson Orin Nano 환경 구축, YOLOv11 및 nanoOWL 실습, 2025
