---
layout: post
comments: true
title : [Basic Clustering_Kmeans]
categories: [TIL]
---

## 군집화 (비지도학습)
###Kmeans?
- 주어진 값들 간의 거리 또는 유사성을 이용하여 분류.
- 전체 데이터를 기준점 중심으로 Euclidean거리가 최소가 되도록 K개의 그룹으로 군집.
- 군집별 중심 값에서 중심과의 거리를 기반으로 데이터를 분류하는 군집기법.

**특징**
- 거리를 이용한 분류
- 반복된 작업 수행
- 짧은 계산 시간
- 주어진 자료에 대한 사전정보 없이 의미 있는 자료구조 찾기 가능
- 범주형(카테고리형) 변수를 다룰 경우 주의

**원리**
- 랜덤으로 초기 K개 군집의 중심이 선택됨.
- 값들간의 거리 비교 후 가까운 군집에 할당함.
- 새로운 군집의 중심을 계산함.
- 재정의된 중심값 기준으로 다시 거리기반의 군집 재분류가 이루어짐.
- 경계의 변경이 이루어지지 않을경우에 종료됨.

**K설정법**
- Elbow point 찾기
- Kmeans는 오브젝트와의 거리의 제곱합이 비용함수 -> 응집도
- k의 개수는 증가하지만 비용함수의 차이가 나지않는 부분이 Elbow point


>비지도학습의 특징: 해석에 따라 결과값이 다르다.
- 그럼에도 사용하는 이유? Elbow Point의 k선택을 위한 정답범위를 줄여주기 때문(선택폭을 좁혀줌)