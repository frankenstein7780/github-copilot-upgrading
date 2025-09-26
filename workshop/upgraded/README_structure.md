# upgraded 폴더 구조 설명

`upgraded` 폴더는 레거시(`legacy`) 폴더의 전체 내용을 복사하여 최신화 및 리팩토링을 진행할 공간입니다. 아래는 주요 폴더 및 파일 구조에 대한 설명입니다.

## 최상위 파일 및 폴더
- `MANIFEST.in`: 패키징 시 포함할 파일 목록을 지정합니다.
- `README.rst`: 프로젝트에 대한 설명 문서입니다.
- `distribute-0.6.10.tar.gz`, `distribute_setup.py`: 레거시 Python 패키징 관련 파일입니다.
- `setup.py`: 프로젝트 설치 및 배포를 위한 스크립트입니다.
- `docs/`: 프로젝트 문서화 관련 폴더입니다.
- `guachi/`: 주요 Python 소스 코드가 위치한 폴더입니다.
- `guachi.egg-info/`: 패키징 정보가 담긴 폴더입니다.

## docs/
- `build/`: Sphinx 등으로 빌드된 문서 결과물이 저장됩니다.
- `source/`: 문서의 원본(rst, conf.py 등)이 위치합니다.

## guachi/
- `__init__.py`, `config.py`, `database.py`: 핵심 Python 모듈입니다.
- `tests/`: 단위 및 통합 테스트 코드가 위치합니다.
  - `test_configmapper.py`, `test_configurations.py`, `test_database.py`, `test_integration.py`: 각각의 테스트 파일입니다.

## guachi.egg-info/
- 패키징 및 배포 관련 메타데이터가 저장됩니다.

---

이 폴더는 레거시 코드를 최신 Python 환경에 맞게 업그레이드하고, 테스트 및 문서화, 패키징 구조를 개선하는 작업을 진행하는 공간입니다.