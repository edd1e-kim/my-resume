# my-resume
My Resume WITH Markdown

##  자기소개
* **이름:** 김재훈
* **전공:** 소프트웨어학과
* **학번:** 32211007
* **학습 목표:** 오픈소스개발

## 연락처 및 주소
* **GitHub:** https://github.com/edd1e-kim
* **Email:** kart215@dankook.ac.kr
* **Blog:** https://blog.naver.com/02_eddie

<p align="center">
  <a href="https://github.com/edd1e-kim">
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/>
  </a>
  <a href="mailto:kart215@dankook.ac.kr">
    <img src="https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/>
  </a>
  <a href="https://blog.naver.com/02_eddie">
    <img src="https://img.shields.io/badge/Blog-000?style=social&logo=naver&logoColor=03C75A"/>
  </a>
</p>

## 기술 스택
* **프로그래밍 언어:**
    <img src="https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=white"/>
    <img src="https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white"/>

* **도구 및 플랫폼:**
    <img src="https://img.shields.io/badge/RocksDB-000000?style=for-the-badge&logo=rocksdb&logoColor=white"/>
    <img src="https://img.shields.io/badge/Makefile-000000?style=for-the-badge&logo=gnu-make&logoColor=white"/>
    <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white"/>
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white"/>

* **자료구조 및 알고리즘:**
    <img src="https://img.shields.io/badge/Data_Structures-007ACC?style=for-the-badge"/>
    <img src="https://img.shields.io/badge/Algorithms-B4009E?style=for-the-badge"/>
    * **자료구조:** B+-Tree, Skip List, Linked List, Stack, Queue, Adjacency Matrix/List, Union-Find
    * **알고리즘:** Quick/Merge/Heap Sort, Prim's/Kruskal's (MST), BFS/DFS, Huffman Coding

* **핵심개념:**
    <img src="https://img.shields.io/badge/Performance_Benchmarking-D00000?style=for-the-badge"/>
    <img src="https://img.shields.io/badge/LSM--Tree-4CAF50?style=for-the-badge"/>
    <img src="https://img.shields.io/badge/Bloom_Filter-FF9800?style=for-the-badge"/>
    <img src="https://img.shields.io/badge/Block_Cache-2196F3?style=for-the-badge"/>
    <img src="https://img.shields.io/badge/Dynamic_Memory-7B1FA2?style=for-the-badge"/>

## 프로젝트 경험
### 1. 자료구조 (Data Structures) - C언어 기반 알고리즘 구현
* **소개:** 자료구조 수업의 일환으로 C언어를 사용하여 핵심 알고리즘과 자료구조를 직접 구현하고 성능을 분석하는 팀 프로젝트들을 수행했습니다. 모든 프로젝트는 `Makefile`을 사용하여 모듈식으로 컴파일 및 빌드했습니다.
* **주요 구현 및 분석 내용:**
    * **정렬 알고리즘:**
        * 기본 정렬 (O(n^2)): 버블 정렬, 선택 정렬, 삽입 정렬 구현.
        * 고급 정렬 (O(n log n)): 퀵 정렬, 병합 정렬, 힙 정렬 구현.
        * 데이터셋 크기 변화에 따른 실행 시간을 그래프로 비교 분석.
    * **그래프 알고리즘:**
        * 최소 스패닝 트리(MST): Prim 및 Kruskal 알고리즘 구현.
        * 그래프 탐색: 너비 우선 탐색(BFS) 및 깊이 우선 탐색(DFS) 구현.
        * 응용: DFS/BFS를 활용한 'Connected Component' 탐색 알고리즘 구현.
    * **트리 (Tree):**
        * 이진 연산 트리: 스택을 활용하여 중위 표기법의 산술식을 이진 트리로 변환.
        * 트리 순회: Infix, Prefix, Postfix, Level-order 4가지 방식의 순회 결과 출력 기능 구현.
        * 허만 트리: 문자열 압축을 위한 허프만 코딩을 구현하고, 결과 비트 수를 ASCII 코드와 비교.
    * **선형 자료구조 (응용):**
        * 다항식 계산기: 연결 리스트(Linked List)와 큐(Queue) 두 가지 방식으로 다항식의 덧셈/뺄셈 기능 구현.
        * 행렬 연산: 동적 메모리 할당을 사용한 행렬의 덧셈, 뺄셈, 곱셈, 희소 행렬 및 전치 행렬 변환 기능 구현.

### 2. 오픈소스분석(빅데이터) - C++ 및 RocksDB 성능 분석
* **소개:** C++로 B+-Tree, Skip List 등 핵심 자료구조를 직접 구현하고, 실제 스토리지 엔진인 RocksDB의 내부 동작(블룸 필터, 캐시, 삭제 매커니즘)을 벤치마킹하고 분석하는 프로젝트들을 수행했습니다.
* **주요 구현 및 분석 내용:**
    * **C++ 자료구조 구현:**
        * **B+-Tree:** 키 삽입, 검색, 분할(split) 로직을 포함한 B+-Tree를 C++로 구현.
        * **Skip List:** `Insert`, `Contains`, `Delete`, `Scan` (범위 조회) 연산을 지원하는 Skip List를 C++로 구현.
        * **성능 평가:** Sequential, Uniform, Zipfian 등 7가지 Synthetic Benchmark를 통해 구현된 자료구조의 성능을 정량적으로 측정.
    * **RocksDB 성능 분석:**
        * **Bloom Filter:** 쓰기 패턴(순차/랜덤)이 블룸 필터의 효율(FPR, useful count)에 미치는 영향을 분석.
        * **Block Cache:** Hot/Cold 데이터 접근 시나리오를 설계하여 블록 캐시 유무(On/Off)에 따른 Cache Hit 비율과 처리량(Ops/sec)을 비교.
        * **Heavy-Delete:** 대량 삭제(Heavy-Delete) 작업 후 수동 Compaction 실행이 읽기 성능(특히 P99.99 Tail Latency)에 미치는 영향을 분석.