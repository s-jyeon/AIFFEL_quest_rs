# AIFFEL Campus Online Code Peer Review Templete
- 코더 : 서지연
- 리뷰어 : 강희봉


# PRT(Peer Review Template)
- [x]  **1. 주어진 문제를 해결하는 완성된 코드가 제출되었나요?**
    - 문제에서 요구하는 최종 결과물이 첨부되었는지 확인
        - SentencePiece 이용 모델 구현의 모든 과정 정상적으로 진행됨 (구현부는 캡쳐 생략 )
        - SimpleRNN 모델을 이용하여 sentncePiece 토크나이저와 결합하여 80% 이상의 테스트 accuracy를 달성   
        - SentencePiece 성능을 다각도로 비교 분석하고 다른 토크나이저(KoNLPy okt 형태소 분석기, Mecab)도 비교 분석   
      ![image](https://github.com/user-attachments/assets/d9e48d4d-ea54-49cf-8169-41f6b6a4eb84)    
      ![image](https://github.com/user-attachments/assets/a83987e5-5bbc-480f-b495-8f556dc7b7ee)   

- [x]  **2. 전체 코드에서 가장 핵심적이거나 가장 복잡하고 이해하기 어려운 부분에 작성된 
주석 또는 doc string을 보고 해당 코드가 잘 이해되었나요?**
    - 추가 모델 실험에 주석을 깔끔하게 작성하였습니다   
    ![image](https://github.com/user-attachments/assets/5faa80af-8af1-4e5e-8446-915157f8f92f)   

- [x]  **3. 에러가 난 부분을 디버깅하여 문제를 해결한 기록을 남겼거나
새로운 시도 또는 추가 실험을 수행해봤나요?**
    - 문제 원인 및 해결 과정을 잘 기록하였는지 확인
    - 두가지 다른 토크나이저에 대해 구현해 실험함   
    ![image](https://github.com/user-attachments/assets/0421391b-e3f9-4630-8c98-d7f6f32685bf)   
    ![image](https://github.com/user-attachments/assets/607ddb7f-36bb-4c69-9953-21fa3da4cc04)   

- [x]  **4. 회고를 잘 작성했나요?**
    ![image](https://github.com/user-attachments/assets/76f862fc-46e3-4330-8b8c-462dcdff43cc)

        
- [x]  **5. 코드가 간결하고 효율적인가요?**
    - 예제 코드의 많은 부분을 가져와 사용했으므로 코드는 효율적으로 보이며 text를 사용해 적절히 정리함

# 회고(참고 링크 및 코드 개선)

- vocab 사이즈에 대한 테스트 범위가 달라서 그 부분을 비교해 볼 수 있어서 좋았습니다.
- SentencePiece 외에도 mecab, okt 에 대해서도 실험을 추가로 하셔서 그 부분에서 도움이 되었습니다.


