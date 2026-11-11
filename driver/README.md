# jmk-wifi 드라이버 소스 (GPL-2.0)

jmk-wifi 패키지에 들어 있는 `88x2bu.ko`(Realtek RTL88x2BU USB Wi-Fi 드라이버)를 다시 빌드하는 데 필요한 파일입니다.

| 파일 | 내용 |
|---|---|
| `SOURCE.txt` | 원본 드라이버 주소와 커밋, 패치·커널·툴체인 정보, 빌드된 `88x2bu.ko`의 해시 |
| `patches/` | 원본 드라이버에 적용한 패치 (이름 순서대로) |
| `build.sh`, `inner-build.sh` | 빌드 스크립트 |
| `config_tcc803x.txt` | 빌드에 쓴 커널 설정 |
| `COPYING` | GPL-2.0 전문 |

## 원본 드라이버

https://github.com/cilynx/rtl88x2bu (GPL-2.0), 커밋 `fc158d1f71b9e5dfcd1fccaf4d28725b65086e3b`

## 빌드

Docker가 필요합니다. 이 폴더에서 `./build.sh`를 실행하면 `out/88x2bu.ko`와 `out/SOURCE.txt`가 만들어집니다.

## 라이선스

원본 드라이버와 패치 모두 GPL-2.0입니다(`COPYING`).
