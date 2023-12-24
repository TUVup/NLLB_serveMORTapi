# NLLB_serveMORTapi
nllb-serve가 MORT와 호환 가능하게 app.py를 수정했습니다.

# 사용법
1. nllb-serve\nllb_serve에 app.py를 교체해 주세요.
2. 커스텀 api 주소 설정을 http://localhost:6060/translate 로 해주세요.
3. 사용 가능한 언어 코드는 [이곳](https://huggingface.co/facebook/nllb-200-distilled-600M/blob/main/special_tokens_map.json)에서 볼 수 있습니다.
4. nllb-serve의 기존 기능들도 사용 가능합니다.

# NLLB 모델 교체
nllb-serve는 기본적으로 nllb-200-distilled-600M을 불러옵니다. 더 나은 번역을 위해 1.3B모델로 교체하여 사용하는걸 권장드립니다.
1. app.py의 \#DEF-MODEL-ID 변수의 주석을 제거하면 "facebook/nllb-200-1.3B"를 기본으로 로드합니다.

또는

2. 실행시 다음과 같이 실행합니다.
```
nllb-serve -mi facebook/nllb-200-1.3B
```

---
●[MORT](https://blog.naver.com/killkimno/70179867557)

●[nllb-serve](https://github.com/thammegowda/nllb-serve)
