# 개발 환경 설정

## Ruby 설치

Ruby를 설치하기 위해 `rbenv`와 `brew`를 사용합니다. `rbenv`는 Ruby 버전 관리 도구이며, `brew`는 macOS 패키지 관리자입니다. 아래는 Ruby 설치 방법입니다:

1. **rbenv 설치**: 터미널을 열고 다음 명령어를 실행하여 `rbenv`를 설치합니다:
   ```shell
   $ brew install rbenv
   ```

2. **rbenv 초기화**: `rbenv`를 초기화합니다. 터미널에서 다음 명령어를 실행합니다:
   ```shell
   $ rbenv init
   ```

3. **rbenv 설치 확인**: `rbenv`가 제대로 설치되었는지 확인합니다. 터미널에서 다음 명령어를 실행하면 현재 설치된 Ruby 버전이 표시됩니다:
   ```shell
   $ rbenv versions
   ```

4. **Ruby 설치**: `rbenv`를 사용하여 Ruby를 설치합니다. 터미널에서 다음 명령어를 실행합니다:
   ```shell
   $ rbenv install [원하는 Ruby 버전]
   ```

5. **전역 Ruby 버전 설정**: 설치한 Ruby 버전을 전역으로 설정합니다. 터미널에서 다음 명령어를 실행합니다:
   ```shell
   $ rbenv global [설치한 Ruby 버전]
   ```

6. **Ruby 설치 확인**: Ruby가 제대로 설치되었는지 확인합니다. 터미널에서 다음 명령어를 실행하면 현재 사용 중인 Ruby 버전이 표시됩니다:
   ```shell
   $ ruby -v
   ```

## 텍스트 에디터 선택

Ruby 코드를 작성하기 위해 텍스트 에디터를 선택해야 합니다. 여기서는 Visual Studio Code(VS Code)를 사용하도록 가정하겠습니다. VS Code는 강력한 편집기이며 Ruby 개발에 많이 사용됩니다. 아래는 VS Code 설치 및 Ruby 개발 환경 설정 방법입니다:

1. **VS Code 설치**: [VS Code 공식 웹사이트](https://code.visualstudio.com)에서 운영체제에 맞는 설치 파일을 다운로드하고 설치합니다.

2. **Ruby 확장 설치**: VS Code에서 Ruby 개발을 위해 "Ruby" 확장을 설치합니다. VS Code의 왼쪽 사이드바에서 "확장" 아이콘을 클릭하고 "Ruby"를 검색한 후 설치합니다.

3. **Gem 설치**: 터미널에서 다음 명령어를 실행하여 Rubocop과 관련한 Gem을 설치합니다:
   ```shell
   $ gem install rubocop
   ```

4. **VS Code 설정**: VS Code에서 Ruby 개발 환경을 설정하기 위해 설정 파일(`settings.json`)을 엽니다. 다음 명령어를 실행하여 설정 파일을 엽니다:
   ```shell
   $ code --user-data-dir
   ```

5. **Ruby 확장 설정**: 설정 파일(`settings.json`)에 아래 내용을 추가합니다:
   ```json
   {
     "ruby.rubocop.executePath": "$(rbenv prefix)/bin/rubocop",
     "ruby.format": "rubocop"
   }
   ```

이제 `rbenv`를 통해 Ruby를 설치하고, VS Code를 설치하여 Ruby 개발 환경을 설정했습니다. 이제 `rbenv`를 사용하여 원하는 Ruby 버전을 선택하고, VS Code에서 편리하게 Ruby 코드를 편집하고 실행할 수 있습니다.