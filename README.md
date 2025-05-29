echo "Репозиторий с откатами изменений" > README.md
git add README.md
git commit -m "Добавил README.md"
git push

touch 1.txt
git add 1.txt
git commit -m "Добавил 1.txt"
git push

touch 2.txt
git add 2.txt
git commit -m "Добавил 2.txt"
git push

git reset --hard "хеш коммита"
git push -f origin main

git revert"хеш коммита"
touch 1.txt
mv 1.txt changed1.txt
git add chanded1.txt
git commit -m "Изменил 1.txt на changed1.txt"
git push
