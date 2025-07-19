step-1:
git init
git add index.html
git commit -m "first commit"
git branch -M main
git remote add origin "URL"
git push -u origin main

step-2:
git branch adminbranch
git checkout adminbranch
git add admin.html
git commit -m "admin file commit"
git push -u origin adminbranch

step-3:
git checkout main
git branch managerbranch
git checkout managerbranch
git add manager.html
git commit -m "manager file commit"
git push -u origin managerbranch

step-4:
git checkout main
git branch userbranch
git checkout userbranch
git add user.html
git commit -m "user file commit"
git push -u origin userbranch

step-5:
git checkout main
git merge adminbranch -m "merge admin to main"
git merge managerbranch -m "merge manager to main"
git merge userbranch -m "merge user to main"
git push -u origin main
