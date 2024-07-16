---
description: LLM(Large Language Model)에 대하여 알아보자.
---

# CH01. LLM(Large Language Model)

#### LLM의 정의

대량의 텍스트 데이터를 기반으로 훈련된 인공지능 모델\
자연어(NLP)작업을 수행할 수 있으며, 언어 이해 및 생성에서 높은 성능을 발휘함

#### &#x20;LLM의 특징

* **규모** : 대규모 데이터셋을 통해 훈련되어, 수억 또는 수조개의 파라메터를 가질수 있음
* **언어이해** : 문맥을 이해하고 관련 정보를 처리하는 능력이 뛰어남
* **다양한 작업 수행** : 이미지 해석, 텍스트 생성, 번역, 요약, 질문 응답 등 여러 NLP작업 수행

#### LLM의 종류

LLM모델은 대략 30여 가지가 존재함, 대표적인 것은 다음과 같음

1. **OpenAI**  : GPT&#x20;
   * GPT-4, GPT-3.5 Turbo : 수백억 개의 파라메터 기반으로 훈련
   * GPT-4o : 텍스트, 오디오, 이미지, 비디오등 다양한 입력 처리 (빠르고 비용 효율)
   * 자연어 이해 및 생성에서 뛰어난 성능, 텍스트 완성, 번역, 질문 응답 등 다양한 언어 관련 작업 수행
   * API를 통해 모델의 다양한 사용옵션 제공, fine-tuning 기능 지원
2. **Anthropic** : Claude&#x20;
   * Claude 3 Haiku : 가장 빠르고 소형모델
   * Claude 3 Sonner :  능력과 속도의 균형, Claude 2.1보다 2배 빠르고 높은 품질
   * Claude 3 Opus : 가장 강력하며, 일반 AI 평가 벤치마크에서 우수한 성능 발휘
   * robustness, safety, and value alignment에 중점
   * 다국어 처리, 비전 및 이미지 처리,  Steerability(행동이나 응답을 조절하는 기능), 편의성이 강점
3. **Google** : Gemini, Gemma
   * Gemini 1.5 Pro : 일반성능   최고의 모델, 1M 토큰 Context Length 제공
   * Gemini 1.5 Flash : 속도와 효율성, 비용 최적화를 위해 설계된 경량 모델
   * Gemma : Gemini 기반의 경량 오픈모델, 노트북이나 데스크탑에서 구동 가능
   * 원활한 멀티모달 설계, 텍스트, 이미지, 오디오등 다양한 입력 이해하고 추론 가능
   * 수학, 물리학 같은 복잡한 주제에 능숙, 코딩을 위한 주요 기초모델로 부상
4. **Meta AI** : Llama 3, code Llama
   * Llama : 자연어 이해, 프로그래밍, 수학적 추론, 논리적 사고에 우수한 성능
   * Code Llama : 코드 이해 및 생성, 코드 완성, 버그탐지와   같은 프로그래밍 관련 작업에 최적화&#x20;
5. **Mistral AI** : Mistral, Mixtral
   * Mistal 7B :  73억개의 파라미터 가진 모델,  로컬 및 클라우드 플랫폼에 배포 가능
   * 최근에 급부상하고 있는 프랑스파리에 기반을 둔 AI사
   * 작은 모델에 강력한 성능강조, 일부 모델은 로컬에서 운영 가능,  오픈 가중치 제공으로 제약이 적음

[https://artificialanalysis.ai/](https://artificialanalysis.ai/)에서 각 LLM의 성능, 가격, 속도등 일괄 비교 가능

<figure><img src=".gitbook/assets/image (1).png" alt=""><figcaption><p><a href="https://mindsdb.com/blog/navigating-the-llm-landscape-a-comparative-analysis-of-leading-large-language-models#heading-openai">https://mindsdb.com/blog/navigating-the-llm-landscape-a-comparative-analysis-of-leading-large-language-models#heading-openai</a></p></figcaption></figure>

#### LLM을 이용하여 개발할 수 있는것

* 고객지원 업무를 담당하는봇챗 제작
* 시장조사 및 보고서 작성
* 문장의 요약, 감정분석, 기계 번역, 문장의 분류
* 작사 나 글쓰기와 같은 창작
* 프로그램 code의 버그 체크  및 해결책 제시

#### LLM 개발 도구 - 프레임 워크

1. **LangChain** : 다양한 LLM 애플리케이션을 지원하는 유연한 프레임 워크
   * 다양한 자연어 처리 모델과 API를 연결하고 조합하여 복잡한 애플리케이션 구축
   * LLM을 사용한 대화형 응용 프로그램, 정보 검색, 대화형 에이전트 등을 만드는데 필요한 도구와 프레임워크 제공
   * 챗봇, 대화형 FAQ 시스템, 문서요약등에 사용
2. **LlamIndex** : LLM 기반 검색 및 검색 작업을 위한 데이터 인덱싱 및 검색 전문
   * LLM을 위한 데이터 인덱싱 및 검색 기능 제공하는 라이브러리
   * DB나 문서에서 정보를 효과적으로 검색하고, LLM과 통합하여 사용자 질문에 답변을 생성
   * 정보 검색 시스템, 데이터 기반 질문 응답 시스템
