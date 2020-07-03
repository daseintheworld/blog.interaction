---
title: "Centromere flashing(Mac)"
permalink: /docs/centromere/qmk/
excerpt: ""
last_modified_at: 2020-07-01T09:00:00
# redirect_from:
#   - /docs/intro/
toc: true
classes: default
---
<br><br>
Qmk toolbox (install 파일)
<br><br>
Brew qmk/qmk/qmk
<br><br>
qmk_firmware
<br><br>
//terminal
Qmk setup . (디렉토리에서)
Y (Library 설치)
Y (submodule 설치)
<br><br>
근데 다 필요 없고 repository에서 make centromere:default 하면 됨
<br><br>
어댑터 : reset 버튼을 두번 누르면 dfu 모드
<br><br>
원래의 centromere에서 MCU 종류를 다르게 올려놔서 혼동이 있었음. 제대로된 atmega32u4를 세팅해놓고 컴파일 해야 맞게된다.
<br><br>
다 끝나면 알아서 돌아온다.