- [ ] 1. test 코드는 진짜 진짜 중요함
- [ ] 2. test input 확인하기
- [ ] 3. test output 확인하기
- [ ] 4. metric은 SOTA 에서 사용한 것이나, 일반적으로 많이 사용하는 것들을 찾아서 사용해야 함.  
      (검증된 것을 사용해야 성능을 인정받을 수 있음)  
      - Summarization : Brio/cal_rouge  
- [ ] 5. valid best checkpoint를 사용함
- [ ] 6. Test시 모델 파라미터 업데이트 안되고 있는지 확인해야 함.
      ```python
      
      # propmt 확인 예시
      encoder.prompt_embeddings.weight

      # 일반적인 모델 예시
      for name, param in self.encoder.named_parameters():
        print(name, param.requires_grad)
      
      ```
----------------------------------------------------------------------------------------------------------------------------------
# Train
- [ ] 1. checkpoint 저장시 파일명을 명확하게 해야 나중에 제대로 실험할 때 문제가 없음  
      \t 1-1. Baseline, Dataset # model/samsumPromptT5Small  
      \t 1-2. model/날짜/checkpoint  # model/20230803/samsumPromptT5Small  

