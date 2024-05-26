---
title: vscode import could not be resolved
draft: false
tags:
  - vscode
  - pylance
  - error
  - pyenv
  - virtualenv
---

![[error_import_could_not_be_resolved.png|600]]

멀쩡히 패키지가 있고, 실행도 잘 되는데 임포트 경고가 거슬린다.  
귀찮아서 무시하고 있다가 오늘따라 너무 거슬려서 없애보기로 한다.  

vscode PyLance 환경설정이 필요하단다.  
pyenv virtualenv 를 쓰고 있어서,  
해당 패키지를 PyLance 가 잡아내지 못하기 때문이다.  

`.vscode/settings.json` 을 추가하라는데,  
사용자계정의 루트 디렉토리가 아닌, (`~/`)  
작업 프로젝트의 루트 디렉토리에 추가하면 된다.  
(`myprj/.vscode/settings.json`)  

python 버전이 3.11.0 이고,  
가상환경 이름이 'pml' 일 때,  
가상환경 하위에 설치된 패키지 주소를 넣으면 된다.  

```json
{
	"python.autoComplete.extraPaths": [
		"~/.pyenv/versions/3.11.0/envs/pml/lib/python3.11/site-packages",

	],
	"python.analysis.extraPaths": [
		"~/.pyenv/versions/3.11.0/envs/pml/lib/python3.11/site-packages"
	]
}
```
 
## 참고 

vscode import could not be resolved - Google Search (google.com) | [Link](https://www.google.com/search?q=vscode+import+could+not+be+resolved&oq=vscode+Import+&sourceid=chrome&ie=UTF-8) 
- Import could not be resolved [Pylance] : r/vscode (reddit.com) | [Link](https://www.reddit.com/r/vscode/comments/o67qm5/import_could_not_be_resolved_pylance/) 
- pylance-release/TROUBLESHOOTING.md at main · microsoft/pylance-release (github.com) | [Link](https://github.com/microsoft/pylance-release/blob/main/TROUBLESHOOTING.md#unresolved-import-warnings) 
- How can I set pylance to use virtual python environment · Issue #330 · microsoft/pylance-release (github.com) | [Link](https://github.com/microsoft/pylance-release/issues/330) 
- pyenv/pyenv-virtualenv: a pyenv plugin to manage virtualenv (a.k.a. python-virtualenv) (github.com) | [Link](https://github.com/pyenv/pyenv-virtualenv?tab=readme-ov-file#usage) 