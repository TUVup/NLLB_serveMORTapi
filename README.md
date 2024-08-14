# NLLB_serveMORTapi
nllb-serve가 MORT와 호환 가능하게 app.py를 수정했습니다.

# 사용법
1. nllb-serve\nllb_serve에 app.py를 교체해 주세요.
2. 커스텀 api 주소 설정을 http://localhost:6060/translate 로 해주세요.
3. 사용 가능한 언어 코드는 [이곳](https://huggingface.co/facebook/nllb-200-distilled-600M/blob/main/special_tokens_map.json)에서 볼 수 있습니다.
4. nllb-serve의 기존 기능들도 사용 가능합니다.

# NLLB 모델 교체
디폴트 모델을 facebook/nllb-200-distilled-1.3B로 바꾸었습니다.

실행시 nllb-serve -mi [model] 방식으로 실행하면 모델을 교체해서 실행가능합니다.

예)
```
nllb-serve -mi facebook/nllb-200-1.3B
```

---
●[MORT](https://blog.naver.com/killkimno/70179867557)

●[nllb-serve](https://github.com/thammegowda/nllb-serve)
