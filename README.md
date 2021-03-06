


## 목차

* [문제의식](#문제의식)

* [블록체인](#BLOCK_CHAIN)
    * [무결성](#무결성)
    * [원장의 순수 P2P 시스템](#원장의 순수 P2P 시스템)
* [비트코인 용어정리](#비트코인 용어정리)
    * [암호화기법](#암호화기법)
    * [보안기술](#보안기술)
    * [아토믹스왑](#아토믹스왑)
    * [라이트닝네트워크](#라이트닝네트워크)


=================
# BLOCK_CHAIN
**무결성을 확보하고 유지하기 위해** 순서에 따라 연결된 블록들의 정보내용을 **암호화 기법과 보안기술을 이용해 협상하는 알고리즘**으로 구성된 소프트웨어 요소를 활용하는 **원장의 순수 분산 P2P시스템**

* 무결성
* 원장의 순수 P2P 시스템
* 암호화기법
* 보안기술


---


## 무결성

시스템이 의도한 대로 작동하는 것

(보안과 정확성을 포함하는 개념)
    
    데이터 무결성: 시스템에서 사용하고 유지 관리하는 데이터는 완전하고 정확하며 모순이 없다
    
    작동 무결성: 의도한 대로 작동, 논리적 오류가 없는 것
    
    보안: 시스템은 허가받은 사용자에게만 데이터 및 기능에 대한 접근 권한을 부여할 수 있다.


사용자에게 응용계층의 기능적 측면 (ex, 사진촬영, 전화, 검색, etc..)의 무결성은 당연하다

-> 해킹, 오류, 버그 등 으로 인한 무결성 파괴

구현 계층의 비기능적 무결성을 지키는 것이 중요함.
> 유저가 당연하게 생각하는 기능을 위해서 무결성을 지키는 것은 중요하다

## 원장의 순수 P2P 시스템

구현 계층의 기능적 측면을 순수 분산시스템으로 구성한 것

    피어(peer), 사용자: 일대 일의 의미, 특정 행위를 하는 사람의 관점
    
    노드(node): 전체 시스템 내 한 요소

    컴퓨터(computer): 공유하는 자원 측면


![centralised VS decentralised](https://maidsafeplatform.files.wordpress.com/2016/01/networksv4.png)

    decentraliztion
    
    장점
    * 계산 능력이 더 뛰어나다
    * 비용이 절감된다
    * 더 안정적이다
    * 자연스럽게 확장이 된다

    단점
    * 조정 오버헤드가 발생한다
    * 통신 오버헤드가 발생한다
    * 네트워크 의존도가 높다
    * 프로그램이 복잡해진다
    * 보안에 신경써야 한다

> 더 많은 사용자가 사용할수록 시스템은 더 거대해지며고 더 강력해진다. 


## 암호화기법

sha-256 

블록생성

해쉬덕후


## 보안기술

블록생성을 쉽지 않게 한다 -> 시간이 오래 걸리게 한다 -> 블록생성의 비용상승

직전 블록의 정보를 가지고 있는다. (직전블록의 해쉬값 보유)

### P2P == 개인과 개인 == 직접거래 == 중개자가 없음
신뢰를 보증하기 위해서는 많은 비용이 발생함.

ex) 국가간자금이체: 간단한 거래의 경우에도 여러 중개자가 개입되어 있으며 처리단계마다 시간과 수수료가 발생

    블록체인은이 전자화폐기술로 주목받는 이유 ?
    중개자 없는 소유권이전에서 무결성을 보증하기 때문
    == 시간과 비용의 절감

### 탈중개화를 위한 유력한도구
순수분산시스템에서는 모든 노드는 동일한 과제를 수행하며, 자원과 서비스의 생산자인 동시에 소비자의 역할을 하게됨

> 탈중개화는 전체 산업 생태계를 변화시킬 상업적 잠재력이 있음


## 어떤 산업을 변화 시킬 것인가?

---
# 비트코인 용어정리
비트코인 구성요소 https://steemkr.com/kr/@yahweh87/3

### 컨센서스(Consensus)
> 합의: 서로 다른 노드들이 생성될 블록에 대해 합의하는 것
> 컨센서스알고리즘(ConsensusAlgoridm): 블록생성 방법에 대한 알고리즘

 악의적인 상황이 발생하더라도 네트워크를 올바른 방향으로 이끌고자하는 다수의 노드들이 상호 검증을 거쳐 올바른 블록 생성을 이끌어내는 프로세스와 알고리즘을 바로 컨센서스(합의)

    http://cointalk.co.kr/bbs/board.php?bo_table=beginner&wr_id=9157

### 컨펌(confirm)
> 트랜젝션이 블록에 포함되는 상황
https://steemit.com/kr/@twinbraid/confirm


### 6컨펌
> 블록이 체인에 완전히 포함된 상태를 인정하는 컨펌숫자

### 0컨펌
> 블록에 포함될 올바른 거래라는 것만 검증하고 승인해주는 것을 말합니다.
https://steemit.com/kr/@twinbraid/42ksz5

### 가장긴체인


### 하드포크

비캐와 비코 블록생성이 같음 https://blockchair.com/search?q=100000

비캐의 비코 하드포크 지점 (478558) https://news.bitcoin.com/fork-watch-first-bitcoin-cash-block-mined/


### 머클트리(MerkleTree))

> 데이터의 간편하고 확실한 인증

머클트리의 장점 https://jayground8.github.io/what_is_merkle_root/
머클루트 구현코드 https://steemkr.com/kr/@yahweh87/4-merkle-tree-merkle-root 


### HD wallet


### UTXO(unspent transaction output)

> 소비되지 않은 트랙젝션 아웃풋........
> 지갑은 개별 트랙젝션의 합으로 이루어짐.

https://steemit.com/coinkorea/@goldenman/utxo

한 지갑안에 15000원이있다고 할 때 1000원 3장 5000원 2장 500원 2개 100원 10개 가 있다고 할 때, 우리가 인지하는 각 금액의 합을 15000원이라고 하는 것은 utxo에서 각 화폐를 보유한 것의 합계를 15000원이라 생각 하는 것과 같다.
만약, 15000원인 상황에서 1000원 1장을 더 받았다면 1000원짜리 utxo가 생성된 것



### 세그윗(segregated witness)

> 분리된 증인. 거래에서 UTXO의 해당하는 부분을 다른곳으로 옮기는 기술
> 거래의 사이즈를 약75% 줄어든다. UTXO의 크기가 줄어 들수 있음.

https://steemit.com/segwit/@loum/segwit


### 아토믹스왑

### 라이트닝네트워크

라이트닝네트워크 이해하기
[1부](https://medium.com/the-litecoin-school-of-crypto/%EB%9D%BC%EC%9D%B4%ED%8A%B8%EB%8B%9D-%EB%84%A4%ED%8A%B8%EC%9B%8C%ED%81%AC-%EC%9D%B4%ED%95%B4%ED%95%98%EA%B8%B0-1%EB%B6%80-6bcc9d0b9d59)
[2부](https://medium.com/the-litecoin-school-of-crypto/%EB%9D%BC%EC%9D%B4%ED%8A%B8%EB%8B%9D-%EB%84%A4%ED%8A%B8%EC%9B%8C%ED%81%AC-%EC%9D%B4%ED%95%B4%ED%95%98%EA%B8%B0-2%EB%B6%80-88acfac8fd42)
[3부](https://medium.com/the-litecoin-school-of-crypto/%EB%9D%BC%EC%9D%B4%ED%8A%B8%EB%8B%9D-%EB%84%A4%ED%8A%B8%EC%9B%8C%ED%81%AC-%EC%9D%B4%ED%95%B4%ED%95%98%EA%B8%B0-3%EB%B6%80-4ed250626b13)


### 플라즈마
이더리움 플라즈마 https://github.com/Onther-Tech/plasma-korea/blob/master/README.md




= = =


# 채굴방식
채굴 == 블록(Block)을 캐다 == 네트워크를 유지하는 것

비트코인이 몇개가지고 있다.

0.5개 가지고 있다.

-> 전체 네트워크에서의 지분을 뜻함

=> 많이 가지고 있을 수록 네트워크내의 지분이 많아짐

## 채굴? 이자?


## POW vs POS vs DPOS
### POW (proof-of-work)

컴퓨팅파워를 이용해서 어려운 수학문제를 풀면 그에 대한 보상을 주는 방식

컴퓨팅파워 == 그래픽카드 == 단순연산최적화

수학문제 == 해쉬된 값

푸는 방법 == 무조껀 대입


    POW채굴 방식에 대한 자세한 설명
    https://blog.iwanhae.ga/introduction_of_bitcoin/

    비트코인 블록숫자
    https://blockchain.info/ko/block

### POS (proof-of-stake)


    퀀텀 코어지갑
    
    퀀텀 스테이킹 계산기
    https://qtumexplorer.io/qtum-staking-calculator

### DPOS (delegate-proof-of-stake)
블록체인시스템을 유지할 노드에게 권한을 위임(delegate)하는 방식

선출된 노드는 컴퓨팅파워(POW)를 제공함

ex) STEEM, EOS


    증인에 대하여
    https://steemit.com/kr/@mastertri/-2017830t112650432z

    스팀 증인목록
    https://steemd.com/witnesses

--- 


# WebAssemblyPractice

http://webassembly.org/demo/

http://meetup.toast.com/posts/121


##웹 어셈블리

웹어셈블리는 자바스크립트가 아닌 다른 프로그래밍 언어로 작성된 코드를 브라우저에서 실행시키기 위한 방법이다. 

네이티브(c, c++)가 제공하는 환경을 브라우저에서 네이티브에 가까운 속도로 기능(작동)할 수 있도록 해주는 새로운(비교적) 형식의 코드 

가장 큰 이점은 빠른 실행이지만 웹 프로그래밍이 더 이상 자바스크립트만으로 제한되지 않는다는 장점도 있다

> * https://mbebenita.github.io/WasmExplorer/

컴파일 구분
* 자바스크립트
* 웹어셈블리


---


###구현예시 (helloWorld)
* http://www.popit.kr/%EA%B0%9C%EB%B0%9C%EB%B0%94%EB%B3%B4-webassembly-emscripten-asmjs/

>###HexCodeEditor
>https://mbebenita.github.io/WasmExplorer/

>위 예시에서 hello.html을 그대로 실행하면 하단의 에러발생
>    
>     on the web, we need the wasm binary to be preloaded and set on Module['wasmBinary']. emcc.py will do that for you when generating HTML (but not JS)
>     abort("on the web, we need the wasm binary to be preloaded and set on Module['wasmBinary']. emcc.py will do that for you when generating HTML (but not JS)") at Error
> ==> 웹서버에서 실행하면됨 => wasmBinary가 preLoad안됬기 때문?


###Javascript와 WebAssembly 성능 테스트

자바스크립트 성능최적화등의 이유로 자바스크립트가 더 빠른 경우도 있음

>  * http://meetup.toast.com/posts/121


VM유무
바로실행 
VM

LLVM(Low Level Virtual Machine)

C/C++    =>    LLVM    =>    Emscripten    =>    JavaScript


WebAssembly - hello world 어셈블리를 브라우저에 올려보자
http://www.devpools.kr/2017/01/21/webassembly-binaryen-emscripten/

asm.js -> low level api 를 사용 성능향상
Emscripten -> native를 자바스크립트로

##asm.js
http://asmjs.org/

##emscripten
http://kripken.github.io/emscripten-site/docs/getting_started/downloads.html

####which emcc
    $ which emcc
    $ /Users/hon/work/emsdk-portable/emscripten/incoming/emcc
    
    
    
###웹어셈블리를 써야할까?
* https://github.com/nhnent/fe.javascript/wiki/March-20-March-24,-2017
