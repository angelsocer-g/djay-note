
# [Djay Git Note](../git-note.md)

---
## git reset HEAD [file]

### Base

- soft
  - commit 취소
  - staged 상태

      
- mixed ( default )
  - commit 취소
  - unstaged 상태

    
- hard
  - commit 취소
  - 변경내용 삭제
    
### Tip
#### 원격 저장소 commit 삭제
##### [참조 link](https://gmlwjd9405.github.io/2018/05/25/git-add-cancle.html)
1. local 저장소 reset
```bash
git reset HEAD^
git reset HEAD~2
git reset [commitid]
```
2. 원격저장소 강제(-f 옵션) push
```bash
git push origin master -f
```