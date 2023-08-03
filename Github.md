
# Git Conflict (깃 충돌)
**error messege**
```python
Please commit your changes or stash them before you merge.
```
**해결방안**
```python
git fetch --all
git reset --hard origin/master # /branch
git pull origin main # 원격 저장소 
```
----------------------------------------
**error messege**
```python
fatal: Could not reset index file to revision 'origin/main'
```


**해결방안**
```python
git gc
git rm .git/index
git reset
git pull origin main # remote beanch
```
