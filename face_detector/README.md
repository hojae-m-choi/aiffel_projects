# aiffel_projects

코더: 최호재
리뷰어: 이경규

project submission for aiffel
🔑 **PRT(Peer Review Template)**

- [x]  **1. 주어진 문제를 해결하는 완성된 코드가 제출되었나요? (완성도)**
    >  문제에서 요구하는 최종 결과물이 첨부되었는지 확인
    >  문제를 해결하는 완성된 코드란 프로젝트 루브릭 3개 중 2개, 퀘스트 문제 요구조건 등을 지칭 ( 해당 조건을 만족하는 부분의 코드 및 결과물을 캡쳐하여 사진으로 첨부 )

    - ![image](https://github.com/hojae-m-choi/aiffel_projects/assets/154392651/dfe6f6f0-1c50-4031-b3e9-5b5a0c182fbd)
    - ![image](https://github.com/hojae-m-choi/aiffel_projects/assets/154392651/9ac5c19c-e1f7-4ff9-a859-2c03d9ebfd40)
    - ![image](https://github.com/hojae-m-choi/aiffel_projects/assets/154392651/bf37b02c-511b-45b9-94d4-b5789313142c)
    - ![image](https://github.com/hojae-m-choi/aiffel_projects/assets/154392651/9ad97fbc-04e9-452d-b8ed-3665a6cad7e2)
    - ![image](https://github.com/hojae-m-choi/aiffel_projects/assets/154392651/634cb8cf-e89c-4c5c-bfad-dad66fde7b27)

- [x]  **2. 프로젝트에서 핵심적인 부분에 대한 설명이 주석(닥스트링) 및 마크다운 형태로 잘 기록되어있나요? (설명)**
    - [x] 모델 구성과 의도의 설명이 잘 되었는가? SSD의 기본 구조를 파악하며 목표에 맞게 설정하였습니다.
    - [x] 모델을 의도한 바에 적절하게 만들었는가? output으로 face_boxes, face_classes, predictions가 나오도록 SSD모델을 만들었습니다.
    - [x]  Loss 선정 이유 : 모델 학습시 loss에 nan이 나오는 디버깅 문제를 가졌지만 해결하고자 노력하였습니다.

    - ![image](https://github.com/hojae-m-choi/aiffel_projects/assets/154392651/d05fa69b-b401-455b-ac53-c300d292ab2b)
    - ![image](https://github.com/hojae-m-choi/aiffel_projects/assets/154392651/b0a7383c-ccea-4706-99d9-5c78c304ca5a)
    - ![image](https://github.com/hojae-m-choi/aiffel_projects/assets/154392651/b862b511-d687-498e-acae-309a53be064c)
        
- [x]  **3. 체크리스트에 해당하는 항목들을 모두 수행하였나요? (문제 해결)**
    - [x]  데이터를 분할하여 프로젝트를 진행했나요? (train, validation, test 데이터로 구분) : TFRecord 생성시 train, val로 분리하였습니다.
    - [x]  하이퍼파라미터를 변경해가며 여러 시도를 했나요? (learning rate, dropout rate, unit, batch size, epoch 등) : threshold 값을 변경해 가며 실험 하였습니다.
    - [x]  각 실험을 시각화하여 비교하였나요? : cfg의 두가지 loss를 상황에 맞게 변경해가며 시각화로 이미지를 나타내었고, 변경에 따른 차이점을 발견하였습니다.
    - [x]  모든 실험 결과가 기록되었나요? : 실험의 결과, 문제를 가졌던 부분과 다양한 아이디어와 데이터로 진행한 실험 결과를 작성하였습니다.

    - ![image](https://github.com/hojae-m-choi/aiffel_projects/assets/154392651/fec12307-aa5d-4fdf-ac62-41f50d559e01)
    - ![image](https://github.com/hojae-m-choi/aiffel_projects/assets/154392651/9684eedd-7483-460b-8cf4-c9e0e6ac9fd0)
    - ![image](https://github.com/hojae-m-choi/aiffel_projects/assets/154392651/1d8f233a-5f1d-4ceb-9e3e-a03937dc557c)
    - ![image](https://github.com/hojae-m-choi/aiffel_projects/assets/154392651/f6deddf0-414a-4fe2-ab86-473d4be7ae36)
    - ![image](https://github.com/hojae-m-choi/aiffel_projects/assets/154392651/9f87668c-51c8-4e77-8867-992ddead5c4f)
    - ![image](https://github.com/hojae-m-choi/aiffel_projects/assets/154392651/56994a73-fb28-466b-a563-5a9cedfc616a)

- [x]  **4. 프로젝트에 대한 회고가 상세히 기록 되어 있나요? (회고, 정리)**
    - ![image](https://github.com/hojae-m-choi/aiffel_projects/assets/154392651/100f67cb-af09-44eb-9ff2-46d3558ea502)

