multi_merge_test
================

```bash
$ for n in `seq 10000`; do git checkout -b br$n master; echo $RANDOM > $RANDOM$RANDOM$RANDOM$RANDOM; git add .; git commit -m"$RANDOM"; done; git checkout master; brs="`git branch | grep -v master`"; git merge $brs; git branch -D $brs; git rm *; git commit -m"del"
```
