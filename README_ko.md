![dasicPhoto](images/dasicPhoto.jpg)

# DASIC 다식

60-64 좌우대칭 앨리스 배열 스플릿 키보드

키 수 많은 [안식](https://github.com/yuburoll/ANSIC)이라는 농담을 치고 싶었습니다.

솔더링만 지원하는 기판이지만, 조금 제한이 있는 [핫스왑 버젼](hotswapVersion)을 만들어두었습니다.

## Preparation

- 2x 프로마이크로 폼팩터 개발보드

- 2x 다식 PCB 보드, 본 레포지토리에서 제공

- 1x 케이스 출력물 세트, 왼쪽 오른쪽 총 2파츠, 본 레포지토리에서 제공

- 2x 1.5-1.6T 키보드 보강판, 본 레포지토리에서 제공

- 2x 1.5-1.6T 백플레이트, 본 레포지토리에서 제공

- 0-2x 0.5u 블로커, 본 레포지토리에서 제공, 보통 1개

- 64x 다이오드

- 24-34x M2x6 접시머리 나사

- 2x PJ320A 1/8(3.5mm) TRRS 커넥터

- 2x 4x4x1.5mm smd 소형 스위치

- 1x 1/8(3.5mm) TRRS 케이블(TRS도 됩니다)

- 2-6x 무보강용 2u 스태빌라이저, 보통 4개(텐키리스 세트)

- 60-64x MX 키스위치, 보통 62개

- 키캡 세트, 텐키 포함을 추천합니다

## Build Guides

[빌드가이드 보러가기](documents/buildGuide_ko.md)

주의사항 요약은 다음과 같습니다.

- **개발보드를 납땜하기 전에 우선 펌웨어를 개발보드에 올려주세요.**

- 개발보드를 동봉된 2.5mm 높이 핀헤더와 함께 pcb의 앞면에 납땜해주세요. 개발보드 부품이 있는 면이 아래를 향해야 합니다.

- pcb 뒷면의 모든 점퍼를 땜해주세요.

- 납땜 기판을 핫스왑 가능하게 만들고 싶다면 밀맥스 형태의 소켓을 대신 땜해야 합니다.

- 밀맥스를 땜할 땐 캡스락과 엔터 위치에 조심하세요. 뒷면 패드마스크의 중앙에 오도록 해주세요.

## Default Keymap

![dasicKeymap](images/dasicKeymap.png)

fn, num 레이어가 추가로 있습니다. 색깔 각인으로 어떻게 작동하는지 확인하실 수 있습니다. ◇는 기본 키맵의 키를 이용한다는 이야기입니다.

우하단의 fn, num키를 길게 누르면 해당 레이어로 바뀝니다.

키캡을 꼽을 땐 다음 이미지를 참고해주세요.

![dasicKeycap](images/dasicKeycap.png)

## Licenses

모든 코드는 MIT license를 따릅니다.

모든 디자인과 하드웨어 보드는 CC BY-SA 4.0 license를 따릅니다.

본 디자인을 가지고 상업활동을 하고 싶으시다면, 몇 푼 정도 후원해주시면 감사하겠습니다...

![dasicCase](images/dasicCase.png)

![dasicPCB](images/dasicPCB.png)