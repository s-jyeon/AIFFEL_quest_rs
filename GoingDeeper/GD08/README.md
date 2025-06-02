# AIFFEL Campus Online Code Peer Review Templete
- 코더 : 서지연
- 리뷰어 : 강희봉


# PRT(Peer Review Template)
- [x]  **1. 주어진 문제를 해결하는 완성된 코드가 제출되었나요?**
    - KoGPT2와 SFT 적용 모델 결과 분석
    - SFT 모델과 RM 모델 결과 분석 ( PPO )
    - 데이터셋 추가 정제 부분은 generation 성능 향상 기법만 적용되었습니다.
    - 새로운 데이터 수집 후 SFT 적용, RM 적용(시간부족으로 완료 안됨)
    - 정성적 분석 위주, 정량 지표는 RM score.
    - 추가 부분 위주 캡쳐    
![image](https://github.com/user-attachments/assets/7821b827-728d-422c-94fb-67363ba72297)    
![image](https://github.com/user-attachments/assets/38645c38-a6fe-476e-bfc7-72ffda7f40fb)    

    - 결과 기본   
![image](https://github.com/user-attachments/assets/3bd3adb9-4ddc-4b7a-b024-90a2c9929419)   

    - SFT   
![image](https://github.com/user-attachments/assets/5366f3b4-cb6e-4d49-8a8b-b0d793db31f8)    

    - RM    
![image](https://github.com/user-attachments/assets/7c84c6f4-379a-4bbc-8c46-25071ea2908a)    

    - PRO   
![image](https://github.com/user-attachments/assets/a4dbf142-b13c-47e4-9130-2814e0d364c5)   

    - SFT ( 새로운 데이터 수집 )   
![image](https://github.com/user-attachments/assets/40720502-dfea-4511-888f-bf5f9df80b9b)   

    
- [x]  **2. 전체 코드에서 가장 핵심적이거나 가장 복잡하고 이해하기 어려운 부분에 작성된 
주석 또는 doc string을 보고 해당 코드가 잘 이해되었나요?**
    - 모델 훈련과 generation을 어떻게 하느냐가 핵심이라고 생각되는데 해당 부분에 주석처리를 잘하였습니다.
![image](https://github.com/user-attachments/assets/13893993-6c87-44cf-afc2-ae5a8c24f095)
![image](https://github.com/user-attachments/assets/47c7a284-dbc8-4d53-ab1e-c12970cced52)

- [x]  **3. 에러가 난 부분을 디버깅하여 문제를 해결한 기록을 남겼거나
새로운 시도 또는 추가 실험을 수행해봤나요?**
    - 한자어가 계속 나오던 문제 새로운 데이터를 적용한 SFT 에서 해결됨 ( 캡쳐는 1번 참조 )
        
- [x]  **4. 회고를 잘 작성했나요?**
    - 진행 과정에서 문제 해결된 부분과 안된 부분과 원인에 대한 생각 그리고 느낀점을 정리하였습니다.
        
- [x]  **5. 코드가 간결하고 효율적인가요?**
    - 필요한 주석을 적절히 추가 - 캡쳐는 2번 참고 


# 회고(참고 링크 및 코드 개선)
- 전 PRO 까지도 시간이 부족했는데 새로운 데이터 수집까지 진행한 부분이 인상적입니다.
- 시간 관계상 완료하지 못한 RM 및 정량지표를 추가 부분 등은 저도 완료하지 못한 부분이 있어 아쉬움이 남습니다.
