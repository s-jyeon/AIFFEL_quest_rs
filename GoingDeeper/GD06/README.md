# AIFFEL Campus Online Code Peer Review Templete
- 코더 : 서지연
- 리뷰어 : 조성호


# PRT(Peer Review Template)
- [ ]  **1. 주어진 문제를 해결하는 완성된 코드가 제출되었나요?**
    - 학습 가능 파라미터 수가 4M인 BERT 모델을 만들고, 모델에 맞는 학습 데이터를 준비하여 학습이 잘 진행되었다.
    - mlm_loss가 줄지 않는 것처럼 보이나 nsp_loss의 스케일이 너무 커서 확인되지 않은 것이고, 학습 과정에서는 줄어들고 있는 것이 확인된다.

![image](https://github.com/user-attachments/assets/669de089-3cdf-45e8-8f40-f5c4488728cb)

![image](https://github.com/user-attachments/assets/13264122-46bf-43d7-9a36-7a425b56a9fd)

![image](https://github.com/user-attachments/assets/54fb0752-094c-472e-8c46-86c51587dfde)
    
- [ ]  **2. 전체 코드에서 가장 핵심적이거나 가장 복잡하고 이해하기 어려운 부분에 작성된 
주석 또는 doc string을 보고 해당 코드가 잘 이해되었나요?**
    - BERT 모델 구현 과정에서 함수와 클래스의 설명이 잘 되어 있어 복잡한 BERT 모델을 이해하기 쉬웠다.
    - BERT 모델 뿐만 아니라 BERT를 구성하는 다양한 함수들 역시 각 파라미터의 의미가 담겨 있어 이해하기 쉬웠다.
![image](https://github.com/user-attachments/assets/60305b0f-7221-4667-b8df-7bcfe7dd90c1)

![image](https://github.com/user-attachments/assets/59bac294-3921-41f7-a7b8-566e98aa7521)
        
- [ ]  **3. 에러가 난 부분을 디버깅하여 문제를 해결한 기록을 남겼거나
새로운 시도 또는 추가 실험을 수행해봤나요?**
    - 학습한 모델로 인퍼런스를 수행하여 mlm, nsp 문제에서의 결과를 확인했다.
    - nsp 인퍼런스 결과의 내용 중 코드가 잘못되어 해석이 잘못된 부분을 찾아 코더에게 전달하였다.
    - 아래 캡쳐 중 nsp 결과는 is_next 확률이 반전되어 모두 올바른 예측을 수행한 것으로 이해하면 된다.
![image](https://github.com/user-attachments/assets/6cd48e7d-1b1a-486c-aee3-3f54f57787e8)

![image](https://github.com/user-attachments/assets/9f47627a-73db-4ba3-8310-e996f7b21290)

        
- [ ]  **4. 회고를 잘 작성했나요?**
    - 회고는 시간 안에 작성하지 못한 것으로 보인다.
        
- [ ]  **5. 코드가 간결하고 효율적인가요?**
    - 모델 구성에 필요한 함수들을 선언하고, bottom up 방식으로 필요한 층을 하나씩 만들어 가며 최종 BERT 모델을 구성하였다.
![image](https://github.com/user-attachments/assets/035eb728-c0e4-4cc2-935f-5e70341e4e38)

![image](https://github.com/user-attachments/assets/e375afa1-387f-44f2-b021-08b292c6cfbe)

![image](https://github.com/user-attachments/assets/a89302d9-3953-4e2b-81d3-c6c05cddfc8d)

![image](https://github.com/user-attachments/assets/2cbe5764-8774-4b0b-91f0-aac15474ab0d)

# 회고(참고 링크 및 코드 개선)
```
하이퍼 파라미터 값을 수정하여 더 작은 모델로 학습을 진행했으면 어땠을까 하는 궁금증이 있습니다.
nsp 인퍼런스 코드에서 예측값이 반전되어 출력되는 오류를 발견했습니다.
인퍼런스 입력으로 위키 형식의 문장을 넣으니 예측 정확도가 높다는 것을 확인했습니다.
저는 인퍼런스 입력으로 일반적인 대화를 넣어 진행했는데, 입력을 위키 형식으로 바꿔보고 싶다는 생각을 했습니다.
```

