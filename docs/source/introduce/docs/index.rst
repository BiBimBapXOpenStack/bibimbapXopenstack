글 작성 방법
============
스터디 블로그에 글을 작성하는 방법입니다.

1. 저장소 가져오기
-----------------------------

- git clone 명령어를 통해 레포지토리를 가져옵니다.

- 먼저 bibimbapXopenstack 레포지토리를 작업할 로컬환경으로 clone을 통해 가져오는 작업입니다.

.. code-block:: console

    > git clone git@github.com:BiBimBapXOpenStack/bibimbapXopenstack.git

- clone 을 통해 가져온 폴더로 들어간 뒤 해당 경로로 이동합니다

.. code-block:: console

    > cd bibimbapXopenstack/docs/source
    
2. 작업하기
-----------------------------

- 해당 디렉토리 중 자신이 속한 팀의 디렉토리로 이동한 뒤 작성할 내용들을 작성해줍니다

.. code-block:: console

    > cd team1
    > ...

3. 새로운 브랜치에서 커밋후 푸쉬하기
-----------------------------

- 모든 작업이 끝났다면 자신의 이름의 브랜치로 이동합니다

.. code-block:: console

    > git checkout -b team1/jaemin # team1/jaemin을 자신의 팀/자신의 이름으로 변경해야 합니다.

- 해당 브랜치로 커밋을 진행합니다

- 커밋메시지 : [TEAM1/jaemin] : 로드밸런싱 과제부분 수정

- 커밋메시지 형식을 지켜서 커밋해주시면 감사하겠습니다.(TEAM1/jaemin도 마찬가지로 자신의팀/이름 으로 변경해야 합니다.)

- 커밋 후 origin으로 푸쉬합니다.

.. code-block:: console

    > git push origin jaemin

4. Pull Request 생성
-----------------------------

- github repository로 들어와 pr을 생성해줍니다

- pull request 본문에는 작업한 내용들을 리스트로 작성해줍니다.

- 이후 pull request를 생성한 뒤 build_check가 모두 이루어질 때까지 기다립니다.

5-1. build_check 성공시
------------------------------

- merge 는 스터디 관리자분들이 진행하기 때문에 여기까지 하시면 완료압니다.

5-1. build_check 실패시
------------------------------

- 빌드 체크에 실패할 경우 detail 버튼을 통해 빌드 상세 정보로 들어갑니다

- 내리다보면 에러가 뜬 부분이 있을텐데 참고하셔서 수정하시면 됩니다

- 빌드 테스트에 통과하지 못한 pull request는 merge없이 close 해주시면 됩니다


