
# [Djay Git Note](../git-note.md)

---
## git config

### Base

- global
  - global
- local
  - git 저장소별 config (global보다 우선)
    
### Tip
#### config list 조회
- list
```bash
git config --list
git config --list --global
git config --list --local
```  
#### config 설정 set
- set name, email
```bash
git config --local user.name "djay.yim"
git config --local user.email "angelsocer@gmail.com"
```

#### config 설정 삭제(unset)
- unset name, email
```bash
git config --unset --local user.name
git config --unset --local user.email
```