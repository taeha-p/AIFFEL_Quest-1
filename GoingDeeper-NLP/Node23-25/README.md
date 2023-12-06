Aiffel에서 진행한 GoingDeeper 노드관련 코드들입니다!

----

STEP 1. NSMC 데이터 분석 및 Huggingface dataset 구성   
- 데이터셋은 깃허브에서 다운받거나, Huggingface datasets에서 가져올 수 있습니다. 앞에서 배운 방법들을 활용해봅시다!    

STEP 2. klue/bert-base model 및 tokenizer 불러오기    
STEP 3. 위에서 불러온 tokenizer으로 데이터셋을 전처리하고, model 학습 진행해 보기   
STEP 4. Fine-tuning을 통하여 모델 성능(accuarcy) 향상시키기   
데이터 전처리, TrainingArguments 등을 조정하여 모델의 정확도를 90% 이상으로 끌어올려봅시다.     

STEP 5. Bucketing을 적용하여 학습시키고, STEP 4의 결과와의 비교    
아래 링크를 바탕으로 bucketing과 dynamic padding이 무엇인지 알아보고, 이들을 적용하여 model을 학습시킵니다.   

Data Collator   

Trainer.TrainingArguments 의 group_by_length   

STEP 4에 학습한 결과와 bucketing을 적용하여 학습시킨 결과를 비교해보고, 모델 성능 향상과 훈련 시간 두 가지 측면에서 각각 어떤 이점이 있는지 비교해봅시다.   

----


코더 : 김지원    

리뷰어 : 

🔑 **PRT(Peer Review Template)**

- [ ]  **1. 주어진 문제를 해결하는 완성된 코드가 제출되었나요?**

    
- [ ]  **2. 전체 코드에서 가장 핵심적이거나 가장 복잡하고 이해하기 어려운 부분에 작성된 
주석 또는 doc string을 보고 해당 코드가 잘 이해되었나요?**

        
- [ ]  **3. 에러가 난 부분을 디버깅하여 문제를 “해결한 기록을 남겼거나” 
”새로운 시도 또는 추가 실험을 수행”해봤나요?**

        
- [ ]  **4. 회고를 잘 작성했나요?**


- [ ]  **5. 코드가 간결하고 효율적인가요?**


Reference:

