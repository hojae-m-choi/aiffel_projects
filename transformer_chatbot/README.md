🔑 **PRT(Peer Review Template)**

- [o]  **1. 주어진 문제를 해결하는 완성된 코드가 제출되었나요? (완성도)**
    - 문제에서 요구하는 최종 결과물이 첨부되었는지 확인
    - 문제를 해결하는 완성된 코드란 프로젝트 루브릭 3개 중 2개, 
    퀘스트 문제 요구조건 등을 지칭
        - 해당 조건을 만족하는 부분의 코드 및 결과물을 캡쳐하여 사진으로 첨부

<img width="845" alt="스크린샷 2024-06-20 오후 5 53 49" src="https://github.com/coronarita/aiffel_projects/assets/101229388/d19e139f-a98a-4dae-a0ce-60f28b604a93">
<img width="718" alt="스크린샷 2024-06-20 오후 5 54 09" src="https://github.com/coronarita/aiffel_projects/assets/101229388/8f4755e4-de87-4ef7-8ecc-c1ea3b62ebe1">
<img width="644" alt="스크린샷 2024-06-20 오후 5 54 36" src="https://github.com/coronarita/aiffel_projects/assets/101229388/9cbb28c6-2d5b-412b-bae1-315ba06cb771">
  > 루브릭 3개중 3개를 만족하였습니다.

- [o]  **2. 프로젝트에서 핵심적인 부분에 대한 설명이 주석(닥스트링) 및 마크다운 형태로 잘 기록되어있나요? (설명)**
    - [o] 모델 구성과 의도의 설명이 잘 되었는가?
    - [o] 모델을 의도한 바에 적절하게 만들었는가?
      > 한국어 문장의 분포를 고려해서 Max_length를 설정하였음
      <img width="418" alt="스크린샷 2024-06-20 오후 5 57 14" src="https://github.com/coronarita/aiffel_projects/assets/101229388/0a79b217-0228-4631-ab14-02597053be5a">
      
    - [ ]  Metrics 선정 이유

    - [o]  Loss 선정 이유
    <img width="937" alt="스크린샷 2024-06-20 오후 5 59 09" src="https://github.com/coronarita/aiffel_projects/assets/101229388/25f1659d-40e3-48ac-8ca7-83e0d9670da7">

- [o]  **3. 체크리스트에 해당하는 항목들을 모두 수행하였나요? (문제 해결)**
    - [o]  데이터를 분할하여 프로젝트를 진행했나요? (train, validation, test 데이터로 구분)
      
    - [o]  하이퍼파라미터를 변경해가며 여러 시도를 했나요? (learning rate, dropout rate, unit, batch size, epoch 등)
      <img width="653" alt="스크린샷 2024-06-20 오후 5 59 26" src="https://github.com/coronarita/aiffel_projects/assets/101229388/23eb8364-ddc2-4efe-924b-1cb0200f553c">

    - [o]  각 실험을 시각화하여 비교하였나요?
    <img width="546" alt="스크린샷 2024-06-20 오후 5 59 40" src="https://github.com/coronarita/aiffel_projects/assets/101229388/bd5e1e14-a2da-41c8-91f7-94fe39d9c43c">

    - [o]  모든 실험 결과가 기록되었나요?
    <img width="697" alt="스크린샷 2024-06-20 오후 5 59 51" src="https://github.com/coronarita/aiffel_projects/assets/101229388/8ad5ab74-a3f0-435d-aae3-811fecda8516">

- [x]  **4. 프로젝트에 대한 회고가 상세히 기록 되어 있나요? (회고, 정리)**
    - [o]  배운 점

    tokenize 해 줄 때, 의미의 단위로 tokenize를 해주는게 중요하다는 것을 확인했다.
    training 시에 validation set 을 꼭 사용하자. 그래야, 몇 epoch 까지 진행해야 할지 판단할 수 있다.

    - [o]  아쉬운 점

    encoder 의 embedding layer, decoder 의 embedding layer 를 분석해보고 싶었으나 시간이 부족해 수행하지 못했다.
    accuracy 외의 다른 지표도 시도해봤으면 좋을것 같다.

    - [o]  느낀 점

    transformer는 학습이 느리다.
    성능을 높이기 위해서 전처리가 중요하다.
    단순히 layer 만 늘려도 성능이 올라가는 경우가 있다.

    - [o]  어려웠던 점

    validation 을 지정하지 않았을 때, 최대 성능이 나오려면 몇 epoch까지 진행해야 할 지 감이 잘 안잡혔다.

<img width="746" alt="스크린샷 2024-06-20 오후 5 56 17" src="https://github.com/coronarita/aiffel_projects/assets/101229388/26bc7789-d253-43d4-9fa5-e2493958b621">
