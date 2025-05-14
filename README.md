# 가상 면접 사례로 배우는 대규모 시스템 설계 기초 ( System Design Interview )

<br>

<br>

# 목차

- [1. 사용자 수에 따른 규모 확장성](https://github.com/KimYongJ/system-design-interview-notes/blob/main/summary/1.%20%EC%82%AC%EC%9A%A9%EC%9E%90%20%EC%88%98%EC%97%90%20%EB%94%B0%EB%A5%B8%20%EA%B7%9C%EB%AA%A8%20%ED%99%95%EC%9E%A5%EC%84%B1.md)

- [2. 개략적인 규모 추정](https://github.com/KimYongJ/system-design-interview-notes/blob/main/summary/2.%20%EA%B0%9C%EB%9E%B5%EC%A0%81%EC%9D%B8%20%EA%B7%9C%EB%AA%A8%20%EC%B6%94%EC%A0%95.md)

- [3. 시스템 설계 면접 공략법](https://github.com/KimYongJ/system-design-interview-notes/blob/main/summary/3.%20%EC%8B%9C%EC%8A%A4%ED%85%9C%20%EC%84%A4%EA%B3%84%20%EB%A9%B4%EC%A0%91%20%EA%B3%B5%EB%9E%B5%EB%B2%95.md)

- [4. 처리율 제한 장치의 설계](https://github.com/KimYongJ/system-design-interview-notes/blob/main/summary/4.%20%EC%B2%98%EB%A6%AC%EC%9C%A8%20%EC%A0%9C%ED%95%9C%20%EC%9E%A5%EC%B9%98%EC%9D%98%20%EC%84%A4%EA%B3%84.md)

- [5. 안정 해시 설계](https://github.com/KimYongJ/system-design-interview-notes/blob/main/summary/5.%20%EC%95%88%EC%A0%95%20%ED%95%B4%EC%8B%9C%20%EC%84%A4%EA%B3%84.md)

- [6. 키-값 저장소 설계](https://github.com/KimYongJ/system-design-interview-notes/blob/main/summary/6.%20%ED%82%A4-%EA%B0%92%20%EC%A0%80%EC%9E%A5%EC%86%8C%20%EC%84%A4%EA%B3%84.md)

- [7. 분산 시스템을 위한 유일 ID 생성기 설계](https://github.com/KimYongJ/system-design-interview-notes/blob/main/summary/7.%20%EB%B6%84%EC%82%B0%20%EC%8B%9C%EC%8A%A4%ED%85%9C%EC%9D%84%20%EC%9C%84%ED%95%9C%20%EC%9C%A0%EC%9D%BC%20ID%20%EC%83%9D%EC%84%B1%EA%B8%B0%20%EC%84%A4%EA%B3%84.md)

- [8. URL 단축기 설계](https://github.com/KimYongJ/system-design-interview-notes/blob/main/summary/8.%20URL%20%EB%8B%A8%EC%B6%95%EA%B8%B0%20%EC%84%A4%EA%B3%84.md)

- [9. 웹 크롤러 설계](https://github.com/KimYongJ/system-design-interview-notes/blob/main/summary/9.%20%EC%9B%B9%20%ED%81%AC%EB%A1%A4%EB%9F%AC%20%EC%84%A4%EA%B3%84.md)

- [10. 알림 시스템 설계](https://github.com/KimYongJ/system-design-interview-notes/blob/main/summary/10.%20%EC%95%8C%EB%A6%BC%20%EC%8B%9C%EC%8A%A4%ED%85%9C%20%EC%84%A4%EA%B3%84.md)

- [11. 뉴스 피드 시스템 설계](https://github.com/KimYongJ/system-design-interview-notes/blob/main/summary/11.%20%EB%89%B4%EC%8A%A4%20%ED%94%BC%EB%93%9C%20%EC%8B%9C%EC%8A%A4%ED%85%9C%20%EC%84%A4%EA%B3%84.md)

- [12. 채팅 시스템 설계](https://github.com/KimYongJ/system-design-interview-notes/blob/main/summary/12.%20%EC%B1%84%ED%8C%85%20%EC%8B%9C%EC%8A%A4%ED%85%9C%20%EC%84%A4%EA%B3%84.md)

- [13. 검색어 자동완성 시스템](https://github.com/KimYongJ/system-design-interview-notes/blob/main/summary/13.%20%EA%B2%80%EC%83%89%EC%96%B4%20%EC%9E%90%EB%8F%99%EC%99%84%EC%84%B1%20%EC%8B%9C%EC%8A%A4%ED%85%9C.md)

- [14. 유튜브 설계](https://github.com/KimYongJ/system-design-interview-notes/blob/main/summary/14.%20%EC%9C%A0%ED%8A%9C%EB%B8%8C%20%EC%84%A4%EA%B3%84.md)

- [15. 구글 드라이브 설계](https://github.com/KimYongJ/system-design-interview-notes/blob/main/summary/15.%20%EA%B5%AC%EA%B8%80%20%EB%93%9C%EB%9D%BC%EC%9D%B4%EB%B8%8C%20%EC%84%A4%EA%B3%84.md)

- [16. 배움은 계속된다](https://github.com/KimYongJ/system-design-interview-notes/blob/main/summary/16.%20%EB%B0%B0%EC%9B%80%EC%9D%80%20%EA%B3%84%EC%86%8D%EB%90%9C%EB%8B%A4.md)

---

<br>

- 시스템 설계시 시스템의 요구사항, 제약사항, 그리고 성능 병목 지점을 잘 이해해야 한다.
- 규모 확장성을 갖춘 시스템을 만들기 위해 필수적인 지식 공부를 해야한다.
- 시스템 설계를 공략하는 단계적 접근법을 공부해야 한다.

<br>
