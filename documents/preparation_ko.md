# 준비물과 구매처

알리익스프레스 링크와 한국에서 구할 수 있는 곳의 링크를 올립니다. 국내에서 구하는 게 더 나은 경우 알리 링크를 굳이 올리진 않습니다.

(2026년 2월 21일 기준입니다. 작동하지 않는 링크가 있을 수도 있습니다.)

다른 좋은 스토어나 다른 좋은 구매처가 있다면 그 쪽을 이용해주세요. 구매 링크는 예시일 뿐이며, 일절 저에게 수익이 들어오지 않습니다...

## 다식 pcb 보드 2장

- JLCPCB에서 맡기면 배송비 포함 25달러 가량에 제조할 수 있습니다. https://jlcpcb.com/

- [거버 폴더](../gubber) 안의 [dasic-gerber.zip(솔더링판)](../gerber/dasic-gerber.zip)이나  [dasicHotswap-gerber.zip(핫스왑판)](../hotswapVersion/gerber/dasicHotswap-gerber.zip)을 다운로드 받아 사이트에 올려주시면 됩니다.

## 보강판과 백플레이트

- JLCPCB에서 FR4 1.6mm HASL(no lead)(중요)를 맡기거나, 3d 프린팅을 직접 하거나(이 두께는 보통 안 해줍니다), 임의의 판재 레이저/cnc커팅점에서 백플레이트와 보강판을 맡깁니다. 각각 원하는 도면으로 구매합니다. 백플레이트와 보강판을 각각 한 쌍씩 준비해주세요.

- JLCPCB에 맡길 땐 거버 폴더[(솔더링판 및 백플레이트)](../case/platesGerber)[(핫스왑판)](../hotswapVersion/HotswapPlate/hotswapPlateGerber) 안의 하위 폴더들에서 원하는 도면의 거버 압축 파일을 다운로드 받아 사이트에 업로드하면 됩니다. https://jlcpcb.com/

- fdm이나 sls 출력을 할 땐 [stl 폴더](../case/stl) 안의 내용물들 중 원하는 사양을 다운로드 받아 출력해주시면 됩니다.

- 레이저/cnc커팅을 맡길 땐 [platesVector 폴더](../case/platesVector) 내에 있는 dxf 파일이나 svg 파일 도면을 전달드리면 됩니다. 원본 사이즈대로 인쇄해달라면 해주실 겁니다.

## 3d 프린팅된 케이스 한 쌍과 0.5u 블로커

- JLC3dp에서 맡기면 약 5~8달러에 한 쪽씩 sls 레진으로 제조해 줍니다. 위의 pcb 보드와 같이 구매해주세요. https://jlc3dp.com/

- 아니면, 직접 fdm 3d 프린팅해서 만들거나 fdm 출력대행을 찾아서 프린팅해 저렴하게 구성해도 좋습니다.

- fdm이나 sls 출력을 할 땐 [케이스 폴더](../case/stl) 안의 내용물들 중 원하는 사양을 다운로드 받아 출력소에 전달해주시면 됩니다.

- fdm 출력에는 bridged라고 표기되어있는 쪽이 좋습니다. 출력물의 뜨는 부분을 고정해주는 브릿지가 있어, 출력물을 견고하게 만들 수 있습니다.

- Tilt4deg라고 적혀져 있는 것은 4도 틸트가 추가로 되어있는 버젼이며, 기존 버젼과 같은 백플레이트를 사용합니다.

- 블로커를 프린팅할 땐 fdm 출력의 경우 BlockerScrew 버젼을 추천합니다. sls의 경우 BlockerHalfScrew를 사용할 수는 있겠으나, 유연성이 없는 재질이라면 BlockerScrew버젼을 사용해 주시기 바랍니다.


## rp2040 pro micro 보드 2개

- 알리: https://ko.aliexpress.com/item/1005009890367599.html
 
- 국내: https://smartstore.naver.com/plumkit/products/12026654291

https://www.nologo.tech/ 이 회사의 rp2040 ProMicro 제품을 상정하고 있습니다. sparkfun의 rp2040 보드도 잘 작동하리라고 생각합니다.

## PJ320A 3.5mm TRRS 커넥터 2개

- 알리: https://ko.aliexpress.com/item/32951864590.html
 
- 국내: https://m.smartstore.naver.com/costec/products/12661336420  5.6mm로 구매해주세요.
  
## (선택) 4x4x1.5mm smd 스위치 2개

- 국내: https://smartstore.naver.com/domekit/products/4315666002

## (핫스왑) MX 핫스왑 소켓 70개

- 알리: https://ko.aliexpress.com/item/1005007232040760.html
 
- 국내1: https://smartstore.naver.com/sagaklabs/products/9090497445

- 국내2: https://smartstore.naver.com/nana-inc/products/8240806382

- 국내3: https://smartstore.naver.com/around_life/products/10187682355

## 다이오드 64개

납땜이 익숙하지 않다면 THT 다이오드를 쓰시는 걸 추천합니다. 니퍼도 준비해 주세요.

- 국내(THT): https://smartstore.naver.com/ic11401/products/618129765
 
- 국내(SMD): https://smartstore.naver.com/sagaklabs/products/9090469658

## M2x6 접시머리 스크류 나사 40개
 
- 국내: https://smartstore.naver.com/riwootool/products/5561795590 옵션 선택에 주의해주세요

## 2u 무보강 스태빌라이저

- 사막 스테빌: https://smartstore.naver.com/morningcraft/products/13072728359

- 체리 스테빌(스냅인): https://smartstore.naver.com/swagkey/products/5700949313

- 체리 스테빌(스크류인): https://smartstore.naver.com/swagkey/products/5134034319

## MX용 키스위치 64개와 키캡 세트

- 평소에 좋아하시는 거 구하시면 됩니다. 왼손의 2u 엄지 키의 존재 때문에, 될 수 있으면 키패드가 포함된 풀배열 키캡을 추천드립니다.

## 눈물 범폰 8~10mm 4개

- 다이소에서 8~10mm짜리 유리 미끄럼 방지 패드나 충격 방지를 찾으면 저렴하게 쓸만한 물건을 구할 수 있습니다.

## 3.5mm TRRS 케이블 1개 (TRS도 됩니다)

- 아무 케이블이든 좋고, 국내에서 쉽게 구하실 수 있을 겁니다.
