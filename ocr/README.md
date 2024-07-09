# aiffel_projects
### 07.09 코드 리뷰
***
### 코더: 최호재
### 리뷰어: 고대현
***
### 총평

코드에 대한 이해도가 높으시고, 코드에 대한 설명을 쉽게 해주셔서 코드가 동작하는 원리에 대해 잘 알게 되었습니다.

뿐만 아니라, 결과물 시각화와 더불어, 결과물이 이렇게 나온 이유에 대해 설명을 잘 해주셔서 이해하기 편했습니다.

또한 모델의 정확도에 대해 시각화를 하셔서 보기 편했습니다.

호재님, 실험하시느라 고생 많으셨습니다 xD
***
project submission for aiffel
🔑 **PRT(Peer Review Template)**

- [X]  **1. 주어진 문제를 해결하는 완성된 코드가 제출되었나요? (완성도)**
    >  문제에서 요구하는 최종 결과물이 첨부되었는지 확인
    >  문제를 해결하는 완성된 코드란 프로젝트 루브릭 3개 중 2개, 퀘스트 문제 요구조건 등을 지칭 ( 해당 조건을 만족하는 부분의 코드 및 결과물을 캡쳐하여 사진으로 첨부 )
    >  모든 루브릭을 충족하셨고, 관련된 시각화 및 결과물을 잘 만들어 주셨습니다.
    > 
    > ![image](https://github.com/hojae-m-choi/aiffel_projects/assets/102419537/75a34e93-a0b5-4e12-8b43-473cc376a158)


- [X]  **2. 프로젝트에서 핵심적인 부분에 대한 설명이 주석(닥스트링) 및 마크다운 형태로 잘 기록되어있나요? (설명)**
    - [X] 모델 구성과 의도의 설명이 잘 되었는가?
    > CTC 손실 함수 구성 및 기타 CRNN 모델 등을 구성하신 이유가 잘 드러나 있습니다.
    > 
    > ![image](https://github.com/hojae-m-choi/aiffel_projects/assets/102419537/a711b5f9-b157-4337-9e13-4a03181d043e)
    - [X] 모델을 의도한 바에 적절하게 만들었는가?
    > 모델을 의도한 바에 따라 적절하게 만들어주셨습니다.
    - [ ]  Metrics 선정 이유
    - [X]  Loss 선정 이유
    > Loss 선정 이유에 대해 잘 언급해주셨습니다. 위의 자료로 갈음합니다.
        
- [X]  **3. 체크리스트에 해당하는 항목들을 모두 수행하였나요? (문제 해결)**
    - [X]  데이터를 분할하여 프로젝트를 진행했나요? (train, validation, test 데이터로 구분)
    > 데이터를 분할하며 프로젝트를 진행하셨습니다.
    > 
    > ![image](https://github.com/hojae-m-choi/aiffel_projects/assets/102419537/1b4fb211-dd24-4388-aaec-28ba30741f06)
    - [X]  하이퍼파라미터를 변경해가며 여러 시도를 했나요? (learning rate, dropout rate, unit, batch size, epoch 등)
    - [X]  각 실험을 시각화하여 비교하였나요?
    > 각 실험을 시각화하여 비교하셨습니다.
    > 
    > ![image](https://github.com/hojae-m-choi/aiffel_projects/assets/102419537/1e6e2ab2-31c0-43e4-96e4-ba0cc16c23dc)
    - [X]  모든 실험 결과가 기록되었나요?
    > 모든 실험 결과가 기록되었습니다.
    > 
    > ![image](https://github.com/hojae-m-choi/aiffel_projects/assets/102419537/81980702-0473-4b8f-9147-6f0914f53fc5)
    > ![image](https://github.com/hojae-m-choi/aiffel_projects/assets/102419537/f7309bd1-17fb-4e44-8a3c-cceb18e4b97c)

- [X]  **4. 프로젝트에 대한 회고가 상세히 기록 되어 있나요? (회고, 정리)**
> 프로젝트에 대한 회고가 상세히 기록되어 있습니다.
> 
> ![image](https://github.com/hojae-m-choi/aiffel_projects/assets/102419537/c04a58bc-8fe2-4da8-9a83-ad44bd8d1ea3)

    - [O]  배운 점
        * PIL Image 객체를 np.array( pil_img) 를 사용하여 numpy ndarray 로 변경하면 자동으로 dimension 이 (h, w, c) 로 바뀜

    - [O]  아쉬운 점
        * Custom Dataset 정의 할 때, outputs = {'ctc': np.zeros([self.batch_size, 1])} 부분의 기능을 늦게 확인하게 되었다.
            * 모델의 결과 ( ctc_loss 값)에 대한 정보를 미리 줄 수 있도록 한 것.
            * lambda 의 결과로 나오는 tensor 는 size 를 알 수 없기에 미리 dataset에서 지정해 주는 것.

    - [O]  느낀 점
        * 이미 학습된 모델을 사용할 때는 기존의 모델이 충분히 쓸 만 한지 (성능) 원하는 작업을 수행하는데 적합한지 확인하고 사용해야 한다.

    - [O]  어려웠던 점
        * 기존에 학습된 모델을 사용하는 과제였다. 기존의 모델이 어떻게 동작하는지, 어떤 학습 데이터가 사용되었는지, 전처리 방법은 어떤지 면밀히 살펴야 했다.
        * 기존 모델은 (h, w, c) 형태의 image tensor 를 입력으로 받았었는데, 이를 확인하기 전까지 입력 dimension 의 순서가 맞지 않아 문자인식이 제대로 되지 않았다.
