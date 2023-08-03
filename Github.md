
# Git Conflict (깃 충돌)
**git pull 했을 때 error messege**
```python
Please commit your changes or stash them before you merge.
```
**해결방안**
```python
git fetch --all
git reset --hard origin/master # /branch
git pull origin main # 원격 저장소 
```
