# Note

Rust의 첫 기여는 [유효하지 않은 링크 수정](https://github.com/rust-lang/rust/pull/138105)이였다. 
그 이후로 테스트 코드 추가, 에러 진단 메시지 수정, 문서화, ICE(Internal Compilation Error) 해결, 
테스트 구조 리팩터링 등등 조금씩 발을 넓혀가기 시작했다. 
그러다보니 자연스럽게 러스트의 `member`가 되고 싶다는 생각이 들었다. 이름 옆에 박힌 `member` 태그가 멋있어보였달까...
그래서 이제는 단순히 Pull Request나 Issue만 생성하는 것을 넘어서 `member`가 할만한 일들을 조금씩 시도해보고 있다. 
예를 들면 새로 올라온 이슈에 라벨링을 한다던가 중복된 이슈를 찾기도하며, 오래전 이슈 살펴보면서 현재 버전에선 해결되었는지
확인해보고 댓글을 남기기도 하였다. 그리고 새로 올라온 PR 구경하면서 개선할 부분들을 남겨보기도 했다. 
러스트 개발자들은 [Zulip](https://rust-lang.zulipchat.com/)을 사용하여 커뮤니케이션을 하는데, 여기도 시간날 때마다 구경을 한다. 
언어 설계, RFC(Request For Comments), MCP(Major Change Proposal, 그 요새 핫한 MCP 서버 아님) 이런 것들에 
대한 회의록도 공개되어 있다. ([lang team](https://hackmd.io/@rust-lang-team), [compiler team](https://hackmd.io/@rust-compiler-team) 
등등 다른 infra, type도 궁금하면 Zulip에서 찾아보시길)

RFC를 생성하는 것도 목표 중 하나이다. 일단 그전에 무엇이 정말 필요할까 부터 고민을 해야한다. 예전에 러스트로 이분탐색 알고리즘
문제를 풀기 위해 `binary_serch` 함수를 사용하다가 이게 값이 여러개 있을 때에는 그중 아무 인덱스만 반환한다는 것을 알았다.
즉 `lower_bound`나 `upper_bound`처럼 젤 작은 인덱스 혹은 젤 큰 인덱스를 반환하는 것이 아니라 그중 입맛에 맞는 것을 반환하는 함수였다.
Python의 `bisect.binary_left`, `bisect.binary_right`나 C++의 `lower_bound`, `upper_bound`와 같이 동작하는 함수가 러스트에는 없다는 것을 
발견하였다. 그래서 '오 내가 이 함수들을 만들어보면 어떨까'라는 생각이 들었었고, 더 검색을 해보았더니 역시 내 고민은
앞서 산 사람들이 벌써 미리 한 고민이라는 것을 깨달았다. 
[Add `lower_bound`, `upper_bound` and `equal_range` for slices where T: Ord to complement `binary_search`](https://github.com/rust-lang/rfcs/issues/2184)
이미 이런 RFC가 올라와있었고 사람들이 토론한 흔적이 남아있었다. 이때 RFC를 처음 알게되었던 것 같다. 해당 RFC의 결론을 한줄 요약하자면
`partition_point`이라는 메서드가 다 커버가 가능하기에 굳이굳이 불필요한 API를 추가할 필요가 없다는 것이 결론이다. 
암튼 RFC를 생성하는 것이 목표다라는 이야기를 하다 여기까지 왔는데(사실 멀리 안옴), 다른 목표는 커밋이다.

원피스에서 로가 칠무해가 되기 위해 100명의 해적의 심장을 해군에 바쳤다. 
<img width="612" height="450" alt="1764515348" src="https://github.com/user-attachments/assets/8a2c35bc-c5b8-4aa0-99d7-6c299d9afee8" />  
그렇다면 나는 100개의 commit을 남김으로써 [rust-lang](https://github.com/rust-lang) 멤버가 될 발판을 마련해야겠다는 목표가 생겼다.
[rust-lang/rust](https://github.com/rust-lang/rust)에 기여한 횟수는 [thanks.rust-lang.org](https://thanks.rust-lang.org/) 사이트에서 쉽게 볼 수 있다. 
2025-11-30 기준으로 현재 27개의 커밋을 남겼고 모든 버전 기준으로 858등에 위치해있다. 기여를 많이 하는것도 좋지만 Rust 언어의 학습도 멈추지 말자. 
기여하다보면 자연스럽게 늘겠지만 착각하지 말고, 자만하지 말자.
