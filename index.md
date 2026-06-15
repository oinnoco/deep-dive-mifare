# 13.56MHz NFC와 MIFARE Classic 딥다이브

이 문서는 13.56MHz NFC 카드, MIFARE 계열, 특히 MIFARE Classic의 인증과 암호화 흐름을 이해하기 위한 짧은 ebook입니다. Flipper Zero 실습은 본인 소유 카드와 통제 가능한 테스트 리더에서 관찰과 학습 목적으로만 다룹니다.

## 목차

1. [서문: 13.56MHz 카드를 이해하기 위한 지도](chapters/01-introduction.md)
2. [13.56MHz 물리 계층](chapters/02-physical-layer.md)
3. [NFC와 ISO/IEC 14443 Type A](chapters/03-iso14443a.md)
4. [MIFARE 제품군 분류](chapters/04-mifare-families.md)
5. [MIFARE Classic 메모리 구조](chapters/05-classic-memory.md)
6. [리더와 카드가 처음 만났을 때](chapters/06-discovery-anticollision.md)
7. [MIFARE Classic 인증 흐름](chapters/07-classic-authentication.md)
8. [Crypto1과 암호화 동작](chapters/08-crypto1.md)
9. [인증 후 명령 처리](chapters/09-post-auth-commands.md)
10. [리더기에서 실제로 처리되는 값들](chapters/10-reader-processing.md)
11. [Flipper Zero로 관찰하기](chapters/11-flipper-observation.md)
12. [Flipper Zero 실습 설계](chapters/12-flipper-labs.md)
13. [MFKey32와 Nested 계열 공격의 개념](chapters/13-key-recovery-concepts.md)
14. [보안 관점 정리](chapters/14-security-guidance.md)
15. [부록: 용어와 참고자료](chapters/15-appendix.md)

## 이미지 자산

이미지가 필요한 설명 지점은 imagegen을 우선 사용했습니다. 현재 생성 도구가 작업공간 파일 경로를 직접 제공하지 않아, 각 챕터에는 아래 파일명을 기준으로 삽입 위치를 표시했습니다.

- `assets/fig-13mhz-coupling.png`: 13.56MHz 리더 코일과 카드 코일의 유도 결합
- `assets/fig-nfc-mifare-layers.png`: 13.56MHz NFC/MIFARE 계층 구조
- `assets/fig-flipper-lab.png`: Flipper Zero 테스트 랩 구성

## 참고자료

- Flipper Zero Documentation, [NFC](https://docs.flipper.net/zero/nfc)
- Flipper Zero Documentation, [Reading NFC cards](https://docs.flipper.net/zero/nfc/read)
- Flipper Zero Documentation, [Recovering MIFARE Classic keys](https://docs.flipper.net/zero/nfc/mfkey32)
- de Koning Gans, Hoepman, Garcia, [A Practical Attack on the MIFARE Classic](https://arxiv.org/abs/0803.2285)
