# NLP-Project-변재현
2026 AI Scientist course NLP Final project

Origin-Aware Agent: Intelligent RAG for Global Product Insights
LLM의 환각(Hallucination)을 줄이기 위해 정보의 근원지(Source Origin)를 추론하고 다국어 쿼리를 확장하는 Advanced RAG 에이전트 프로젝트입니다.
🚀 프로젝트 개요 (Overview)
일반적인 RAG 시스템은 사용자의 언어(한국어)로만 검색을 수행하여, 글로벌 제품이나 최신 기술 이슈에 대해 데이터 밀도가 낮은 한국어 웹 정보에 의존하게 됩니다. 이는 결국 LLM이 부족한 정보를 메우기 위해 환각을 일으키는 원인이 됩니다.
본 프로젝트는 **"정보는 발생지에서 가장 풍부하고 정확하다"**는 가설을 바탕으로, 질문의 키워드를 분석해 정보의 원천 국가를 식별하고 현지 커뮤니티 데이터를 수집하는 Origin-Aware Query Expansion 기술을 구현했습니다.
✨ 주요 기능 (Key Features)
• Reasoning Agent: Chain-of-Thought(CoT)를 통해 질문 속 키워드의 제조국/출시국을 스스로 추론.
• Multi-Query Expansion: 한국어, 영어, 그리고 추론된 현지어를 조합한 다국어 검색 쿼리 생성.
• Source-Specific Retrieval: Reddit, Kakaku, Zhihu 등 해당 도메인의 '성지' 커뮤니티를 타겟팅하여 고밀도 데이터 수집.
• RAGAS Evaluation: Faithfulness, Context Precision 등 정량적 지표를 통해 환각 억제 성능 검증.
🏗️ 시스템 아키텍처 (Architecture)
1. Analysis: 질문의 카테고리와 정보 원천(Source) 식별.
2. Expansion: CoT 기반 다국어/다각도 쿼리 생성.
3. Retrieval: DuckDuckGo를 이용한 글로벌 웹 데이터 수집.
4. Synthesis: 파편화된 정보를 논리적인 리포트 형태로 종합.

💻 코드 사용법 (Usage)
본 프로젝트는 Google Colab 환경에서 Ollama(Llama 3)를 활용하여 최적화되었습니다.

📂 폴더 구조 (Folder Structure)
• main_proposal.ipynb: 프로젝트 전체 로직 및 실험 코드가 포함된 메인 노트북
• README.md: 프로젝트 설명서
