- [ ] 1. test 코드는 진짜 진짜 중요함
- [ ] 2. test input 확인하기
- [ ] 3. test output 확인하기
- [ ] 4. metric은 SOTA 에서 사용한 것이나, 일반적으로 많이 사용하는 것들을 찾아서 사용해야 함.(검증된 것을 사용해야 성능을 인정받을 수 있음)
          - Summarization : Brio/cal_rouge
- [ ] 5. valid best checkpoint를 사용함
- [ ] 6. Test시 모델 파라미터 업데이트 안되고 있는지 확인해야 함.
      ```python

      encoder.prompt_embeddings.weight

      for name, param in self.encoder.named_parameters():
        print(name, param.requires_grad)
      
      ```

