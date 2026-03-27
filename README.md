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

* RGB 채널별로 디스플레이
 ** numpy의 슬라이싱 기능을 이용하여 RGB 채널별로 디스플레이함
  ![image](https://github.com/user-attachments/assets/ccc2645d-2d72-4e5e-86d6-981c79b175ba)

* 이진화
 ** 알고리즘 : 임계값 T보다 큰 화소는 1, 그렇지 않은 화소는 0으로 바꿈. 임계값 결정이 중요함

* 오츄 알고리즘
 ** 이진화를 최적화 문제로 바라봄. 목적함수는 임계값 t의 좋은 정도를 측정함

* 최적화 문제를 푸는 알고리즘
 ** 오츄는 최적화를 구현하는데 낱낱탐색(exhaustive search) 알고리즘 사용
  *** 매개변수 t가 해공간을 구성하는데, 해공간이 작아 낱낱 탐색 가능
  *** L이 256이라면 해공간은 {0,1,2,...255}
 ** 컴퓨터 비전은 문제를 최적화로 푸는 경우가 많음. 해공간이 커서 낱낱 탐색이 불가능하기 때문에 부최적해(sub-optimal solution)를 찾는 효율적인 알고리즘 사용
  *** 스네이크는 탐욕 알고리즘 사용
  *** 역전파 알고리즘(기계학습을 위해 미분하는 알고리즘)은 미분을 사용함  



   
