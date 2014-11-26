gitTask3
========
Список команд:

  mkdir gitHW3
  cd gitHW3
  git init
  nano tsak3.txt
  mv tsak3.txt task3.txt
  git hash-object -w task3.txt
  git update-index --add --cacheinfo 100644 1193319b42f6c2bb09934b092a1da0b533770062 task3.txt
  git write-tree
  echo "Commit Earlvik 1" | git commit-tree 7a5d6a
  nano task3_new.txt
  nano task3.txt
  git hash-object -w task3.txt
  git hash-object -w task3_new.txt
  git update-index --add --cacheinfo 100644 a883faa4fe157578046a4cb2078d9c7128d517fa task3.txt
  git update-index --add --cacheinfo 100644 7e492146395ee4ca9deed650c84f63e2a74abe64  task3_new.txt
  git write-tree
  git read-tree --prefix=gittask 7a5d6a
  git write-tree
  echo "Commit Earlvik 2" | git commit-tree b1c79d -p 468c14
  echo "Commit Earlvik 3" | git commit-tree c01818 -p 91db7d
  git remote add origin https://github.com/Earlvik/gitTask3.git
  echo "a32320c37531f796eacc9955d6217bd88ee0dc9d" > .git/refs/heads/master
  git update-ref refs/heads/master a32320c37531f796eacc9955d6217bd88ee0dc9d
  git push -u origin master
Домашнее задание по Git школы разработчиков HeadHunter. Задание 3
