Aiffel에서 진행한 GoingDeeper 노드관련 코드들입니다!

코더 : 김지원    

리뷰어 : 서민성

🔑 **PRT(Peer Review Template)**

- [ ]  **1. 주어진 문제를 해결하는 완성된 코드가 제출되었나요?**
    - 주어진 문제를 해결하지 못했습니다.
    
- [ ]  **2. 전체 코드에서 가장 핵심적이거나 가장 복잡하고 이해하기 어려운 부분에 작성된 
주석 또는 doc string을 보고 해당 코드가 잘 이해되었나요?**
    - 데이터 증강 관련하여 주석처리가 잘 되어있었습니다.
    - ```
      def lexical_sub(sentence, word_vec):
        # 임베딩 모델 로드
        model = Word2Vec.load('path/to/word2vec/model')
    
        # 입력 문장을 임베딩으로 확장
        embedded_sentence = [model.wv[word] for word in sentence.split()]
        
        # 대체할 단어 선택
        selected_w = random.choice(sentence)
    
        # 대체할 단어와 가장 유사한 단어 찾기
        similar_word = model.wv.most_similar(target_word, topn=1)[0][0]
    
        # 선택한 단어로 대체
        substituted_sentence = sentence.replace(target_word, similar_word)
    
        return substituted_sentence
    

        
- [ ]  **3. 에러가 난 부분을 디버깅하여 문제를 “해결한 기록을 남겼거나” 
”새로운 시도 또는 추가 실험을 수행”해봤나요?**
    - 에러가 난 부분에 대한 기록을 찾지는 못했습니다.
        
- [ ]  **4. 회고를 잘 작성했나요?**
    - 회고에 대한 기록을 찾을 수 없었습니다.

- [ ]  **5. 코드가 간결하고 효율적인가요?**
    - 코드가 간결하고 효율적으로 작성되었습니다.

Reference:
1. https://iambeginnerdeveloper.tistory.com/41
2. https://velog.io/@seolini43/%ED%8C%8C%EC%9D%B4%EC%8D%ACTransformer%EB%A1%9C-%EC%98%A4%ED%94%BC%EC%8A%A4-%EC%B1%97%EB%B4%87-%EB%A7%8C%EB%93%A4%EA%B8%B0-%EC%BD%94%EB%93%9C
3. https://wikidocs.net/89786
