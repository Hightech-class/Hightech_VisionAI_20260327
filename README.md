# Hightech_VisionAI_20260327
---
* 디지털 영상처리
  ** 영상처리 : 특정 목적을 달성하기 위해 원래 영상을 새로운 영상으로 변환
  ** 컴퓨터 비전은 전처리로 활용하여 인식 성능을 향상

* 핀홀 카메라 모델

* 디지털 변환
  ** M*N 영상으로 샘플링(sampling)
  ** L 단계로 양자화(quantization)
![image](https://github.com/user-attachments/assets/15d6f4f1-1a2e-462c-a1e8-4eb98153eb0a)
 
* 영상 좌표계
 ** 왼쪽 위 구석이 원점 , (y,x)표기
 ![image](https://github.com/user-attachments/assets/95ae508b-e27c-4006-a1bd-f45844594e12)

* OpenCV는 numpy.ndarray로 영상을 표현함
 ** numpy.ndarray가 지원하는 다양한 함수를 사용할 수 있음 (min, max, argmin, argmax, mean, sort, reshape, transpose,.....)
