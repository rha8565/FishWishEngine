# Fishwish 엔진 설치 방법입니다.

## **Setup 순서**<br>
- Repository 내려받기
- 비주얼 스튜디오 다운로드
- 엔진소스 프로젝트 제너레이트
- 엔진 소스 빌드
- 퍼포스와 연결
<br/><br/><br/>

## **Repository 내려받기**
<br>
- 진행전 새로운 Perforce 프로젝트용 폴더를 원하시는 경로에 만듭니다.
- V:\FishWish\03_Unreal\FishWishEngine 경로의 Zip 파일을 perforce 프로젝트 폴더에 압축해제합니다.
<br/><br/><br/>

## **비주얼 스튜디오 다운로드**
- [UE docs Visual Studio 구성하기](https://dev.epicgames.com/documentation/ko-kr/unreal-engine/setting-up-visual-studio-development-environment-for-cplusplus-projects-in-unreal-engine)를 참고하여 VisualStudioSetup.exe를 실행
  비주얼 스튜디오를 다운로드합니다.
<br/><br/><br/>

## **엔진소스 프로젝트 제너레이트**<br/>
<img src="SetupBatch.PNG">
- Perforce프로젝트폴더/UnrealEngine_FishWish/Setup.bat 배치파일을 실행합니다.
  (Setup파일은 여러개 그 중 Windows 배치파일을 실행해야 합니다. 10~30분정도 걸립니다.)
<br/>
<img src="GenerBat.PNG">
- 모두 완료되면 GenerateProjectFiles.bat 파일을 실행합니다.(1분 소요)
<br/><br/><br/>

## **엔진 소스 빌드**<br/>
<img src="UE5_Sln.PNG">
- UE5.sln파일을 실행합니다.(로그인 안하셔도 됩니다.)<br/>
- 오른쪽 솔루션 탐색기에서 Engine->UE5를 우클릭하신후 빌드를 눌러주세요.(오래걸림)<br/>
- 완료되면 "퍼포스프로젝트경로\UnrealEngine_FishWish\Engine\Binaries\Win64\UnrealEditor.exe"를 실행하여 작동이 되는지 확인합니다.<br/>
   (섀이더 컴파일 진행하면 성공)<br/>
- 문제 발생시 개발자를 부르세요.<br/>
<br/><br/><br/>

## **퍼포스와 연결**<br/>
<img src="RemoveList.PNG">
- 우선 위의 파일들을 삭제합니다 (마크다운 정크파일, 설치파일)<br/>
- "V:\FishWish\03_Unreal\PerforceRoot_0411" 경로의 FishWish 루트폴더를 Perforce 프로젝트 폴더 경로로 복사합니다.<br/><br/>
<img src="PerforceSetting.PNG">
- 작업한 폴더를 새로운 Perforce 워크스페이스로 만듭니다.<br/>
- Get Latest를 눌러 프로젝트를 퍼포스와 동기화 시킵니다.<br/>
- AIX2-욱진, AIX3-영주, AIX4-수현<br/>
<br/><br/>
<img src="SwitchEngine.PNG">
- FishWish.uproject를 우클릭한 후 Switch Unreal Engine Version...을 클릭하여 FishWish엔진으로 선택되어있는지 확인합니다.
- 확인 후 프로젝트를 실행합니다. 정상작동한다면 성공

# 문제가 생기면 개발자를 불러주세요 고생하셨습니다. 
