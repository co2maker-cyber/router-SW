# 포트북: 라우터·스위치 인터페이스 대장

Packet Tracer처럼 네트워크 장비·포트·IP·케이블을 기록하는 웹앱입니다. HTML 파일 하나로 되어 있고 따로 설치할 것이 없습니다.

## 실행

`portbook.html`을 내려받아 브라우저로 열면 됩니다. 데이터는 그 브라우저의 localStorage(`portbook.local`)에 저장됩니다.

## 주요 기능

- **토폴로지 / 랙 / 목록 / CLI** 네 화면
- 라우터 25종 실물 뒷면 배치, 모듈 슬롯에 꽂기
- Packet Tracer `.pkt` / `.pka` 파일 불러오기 (파일 메뉴)
- 장비 창: Physical · Config · Attributes
  - 라우터·스위치 Config: Settings, Static·RIP, VLAN Database, 인터페이스 (IOS 명령으로 실행)
  - PC·서버 Config: 게이트웨이·DNS, NIC IP·마스크·포트 상태 (`ipconfig` 명령으로 실행)
- IOS CLI (hostname, interface, ip address, switchport, encapsulation, ip route, router rip 등)와 PC Command Prompt (`ipconfig`, `ping`, `tracert`)
- 케이블·VLAN·게이트웨이·라우팅을 따져 보는 ping / tracert 모의

## 한계

- ping 모의는 캡슐화 불일치, ACL, NAT, DHCP를 반영하지 않습니다.
- `.pkt`에서 Hub·Cloud처럼 "Port 0" 식 이름의 포트에 연결된 케이블, 콘솔·무선 연결은 가져오지 않습니다.
