# [Ch1 한눈에 보는 머신러닝] 연습문제
1. 머신러닝을 어떻게 정의할 수 있나요?
- 머신러닝은 데이터로부터 학습할 수 있는 시스템을 만드는 것
2. 머신러닝이 도움을 줄 수 있는 문제 유형 네 가지를 말해보세요.
- 명확한 해결책이 없는 복잡한 문제
- 수작업으로 만든 긴 규칙 리스트를 대체하는 경우
- 변화하는 환경에 적응하는 시스템을 만드는 경우
- 사람에게 인사이트를 제공해야 하는 경우(ex.. 데이터마이닝)
3. 레이블된 훈련 세트란 무엇인가요?
- 각 샘플에 대해 정답을 담고 있는 훈련 세트
4. 가장 널리 사용되는 지도 학습 작업 두 가지는 무엇인가요?
- 회귀와 분류
5. 보편적인 비지도 학습 작업 네 가지는 무엇인가요?
- 군집, 시각화, 차원 축소, 연관 규칙 학습
6. 사전 정보가 없는 여러 지형에서 로봇을 걸어가게 하려면 어떤 종류의 머신러닝 알고리즘을 사용해야 하나요?
- 강화 학습
7. 고객을 여러 그룹으로 분할하려면 어떤 알고리즘을 사용해야 하나요?
- 그룹을 어떻게 정의할지 모른다면 비슷한 고객끼리 군집으로 나누기 위해 군집 알고리즘(비지도 학습)을 사용할 수 있음
- 어떤 그룹이 있어야 할지 안다면 분류 알고리즘(지도 학습)을 사용할 수 있음
8. 스팸 감지의 문제는 지도 학습과 비지도 학습 중 어떤 문제로 볼 수 있나요?
- 지도 학습
9. 온라인 학습 시스템이 무엇인가요?
- 온라인 학습 시스템은 배치 학습 시스템과 달리 점진적으로 학습할 수 있음  
  이 방식을 사용하면 변화하는 데이터와 자율 시스템에 빠르게 적응하고 매우 많은 양의 데이터를 훈련시킬 수 있음
10. 외부 메모리 학습이 무엇인가요?
- 외부 메모리 알고리즘은 컴퓨터의 주메모리에 들어갈 수 없는 대용량의 데이터를 다룰 수 있음  
  외부 메모리 학습 알고리즘은 데이터를 미니배치로 나누고 온라인 학습 기법을 사용해 학습
11. 예측을 하기 위해 유사도 측정에 의존하는 학습 알고리즘은 무엇인가요?
- 사례 기반 학습 시스템은 훈련 데이터를 기억하는 학습  
  새로운 샘플이 주어지면 유사도 측정을 사용해 학습된 샘플 중에서 가장 비슷한 것을 찾아 예측으로 사용
12. 모델 파라미터와 학습 알고리즘의 하이퍼파라미터 사이에는 어떤 차이가 있나요?
- 모델은 하나 이상의 파라미터(ex.. 선형 모델의 기울기)를 사용해 새로운 샘플이 주어지면 무엇을 예측할지 결정  
  학습 알고리즘은 모델이 새로운 샘플에 잘 일반화되도록 이런 파라미터들의 최적값을 찾음  
  하이퍼파라미터는 모델이 아니라 이런 학습 알고리즘 자체의 파라미터(ex.. 적용할 규제의 정도)
13. 모델 기반 알고리즘이 찾는 것은 무엇인가요? 성공을 위해 이 알고리즘이 사용하는 가장 일반적인 전략은 무엇인가요? 예측은 어떻게 만드나요?
- 모델 기반 학습 알고리즘은 새로운 샘플에 잘 일반화되기 위한 파라미터의 최적값을 찾음  
  일반적으로 훈련 데이터에서 시스템의 예측이 얼마나 나쁜지 측정하고 모델에 규제가 있다면 모델 복잡도에 대한 페널티를 더한 비용 함수를 최소화함으로써 시스템을 훈련시킴  
  예측을 만들려면 학습 알고리즘이 찾은 파라미터를 사용하는 모델의 예측 함수에 새로운 햄플의 특성을 주입
14. 머신러닝의 주요 도전 과제는 무엇인가요?
- 부족한 데이터, 낮은 데이터 품질, 대표성 없는 데이터, 무의미한 특성, 훈련 데이터에 과소적합된 과도하게 간단한 모델, 훈련 데이터에 과대적합된 과도하게 복잡한 모델 등
15. 모델이 훈련 데이터에서의 성능은 좋지만 새로운 샘플에서의 일반화 성능이 나쁘다면 어떤 문제가 있는 건가요? 해결책 세 가지는 무엇인가요?
- 이 모델은 훈련 데이터에 과대적합되었을 가능성이 높음  
  과대적합에 대한 해결책은 더 많은 데이터를 모으거나, 모델을 단순화하거나(간단한 알고리즘 선택, 특성&파라미터의 수를 줄임, 모델에 규제를 추가), 훈련 데이터에 있는 잡음 줄이기
16. 테스트 세트가 무엇이고 왜 사용해야 하나요?
- 테스트 세트는 실전에 배치되기 전에 모델이 새로운 샘플에 대해 만들 일반화 오차를 추정하기 위해 사용함
18. 훈련-개발 세트가 무엇인가요? 언제 필요하고 어떻게 사용해야 하나요?
- 훈련-개발 세트는 (모델을 실전에 투입했을 때 사용될 데이터와 최대한 가까워야 하는)검증, 테스트 세트에 사용되는 데이터와 훈련 세트 사이에 데이터 불일치 위험이 있을 때 사용됨  
  훈련 세트의 일부에서 모델을 훈련, 훈련-개발 세트와 검증 세트에서 평가  
  + 모델이 훈련 세트에서는 잘 작동하지만, 훈련-개발 세트에서 나쁜 성능을 낸다면 훈련 세트에 과대적합되었을 가능성이 높음  
    훈련 세트와 훈련-개발 세트 양쪽에서 모두 잘 작동하지만 검증 세트에서 성능이 나쁘다면 훈련 데이터와 검증 및 테스트 데이터 사이에 데이터 불일치가 있을 가능성이 높음  
    검증 및 테스트 데이터에 더 가깝게 되도록 훈련 데이터를 개선해야 함
19. 테스트 세트를 사용해 하이퍼파라미터를 튜닝하면 어떤 문제가 생기나요?  
- 테스트 세트를 사용해 하이퍼파라미터를 튜닝하면 테스트 세트에 과대적합될 위험이 있고 일반화 오차를 낙관적으로 측정하게 됨
  (모델을 출시하면 기대한 것보다 나쁜 성능을 낼 것)
