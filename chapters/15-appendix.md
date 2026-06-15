[목차](../index.md) | 이전: [보안 관점 정리](14-security-guidance.md) | 다음: 없음

# 15. 부록: 용어와 참고자료

## 용어

`13.56MHz`: NFC와 ISO 14443 계열 비접촉 카드에서 흔히 쓰는 고주파 대역.

`RFID`: 무선 주파수 식별 기술 전체를 가리키는 넓은 말.

`NFC`: 13.56MHz 기반 근거리 통신 기술과 생태계.

`ISO/IEC 14443 Type A`: 많은 13.56MHz 카드가 사용하는 비접촉 카드 통신 규격 계열.

`UID`: 카드 식별자. 인증 전 단계에서 관찰될 수 있다.

`ATQA`: Type A 탐색 요청에 대한 카드 응답.

`SAK`: 카드 선택 후 리더가 카드 성격을 판단하는 데 쓰는 응답.

`MIFARE Classic`: 섹터/블록 메모리 구조와 Crypto1을 사용하는 오래된 MIFARE 계열.

`Key A`, `Key B`: MIFARE Classic 섹터 인증에 쓰이는 48비트 키.

`Access Bits`: MIFARE Classic에서 블록별 읽기/쓰기/값 연산 권한을 정하는 비트.

`Sector Trailer`: Key A, access bits, Key B가 저장되는 섹터의 마지막 블록.

`Crypto1`: MIFARE Classic의 독자 stream cipher. 현대 기준으로 취약성이 알려져 있다.

`Nonce`: 인증 과정에서 쓰이는 임시 난수.

`MFKey32`: MIFARE Classic 인증 transcript의 nonce 정보를 이용해 키를 추정하는 알고리즘/도구 계열.

## Mermaid 도표 목록

- 전체 흐름: 1장
- RF field와 load modulation: 2장
- Type A anti-collision: 3장, 6장
- MIFARE 제품군 분류: 4장
- Classic 메모리 구조: 5장
- Classic 인증 시퀀스: 7장
- Crypto1 stream cipher 개념: 8장
- Access bits 권한 흐름: 9장
- 리더/백엔드 판단 구조: 10장
- Flipper 실습 흐름: 12장
- 키 복구 개념 흐름: 13장
- 위험 모델: 14장

## 참고자료

- Flipper Zero Documentation, [NFC](https://docs.flipper.net/zero/nfc)
- Flipper Zero Documentation, [Reading NFC cards](https://docs.flipper.net/zero/nfc/read)
- Flipper Zero Documentation, [Recovering MIFARE Classic keys](https://docs.flipper.net/zero/nfc/mfkey32)
- de Koning Gans, Hoepman, Garcia, [A Practical Attack on the MIFARE Classic](https://arxiv.org/abs/0803.2285)
- NXP, MIFARE product documentation and product family pages

[목차](../index.md) | 이전: [보안 관점 정리](14-security-guidance.md) | 다음: 없음
