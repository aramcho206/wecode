aramcho@Aramui-MacBookPro Desktop % cd test
aramcho@Aramui-MacBookPro test % ls
wecode
aramcho@Aramui-MacBookPro test % cd wecode

aramcho@Aramui-MacBookPro wecode % git init
          <!-- git was initialized at current directory -->

Initialized empty Git repository in /Users/aramcho/Desktop/test/wecode/.git/
aramcho@Aramui-MacBookPro wecode % 

aramcho@Aramui-MacBookPro wecode % git add .
aramcho@Aramui-MacBookPro wecode % git commit -m "this is git test"
[master (root-commit) c545252] this is git test
 Committer: Aram Cho <aramcho@Aramui-MacBookPro.local>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly. Run the
following command and follow the instructions in your editor to edit
your configuration file:

    git config --global --edit

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 14 insertions(+)
 create mode 100644 test.js
    <!-- at this point, "git add . and git commit" was done and it is now ready to push to git hub -->

aramcho@Aramui-MacBookPro wecode % git branch
* master
    <!--  checking which branch currently in -->

aramcho@Aramui-MacBookPro wecode % git branch -M main
      <!-- git branch was switched to main branch -->

aramcho@Aramui-MacBookPro wecode % git branch
* main
aramcho@Aramui-MacBookPro wecode % git branch
* main
aramcho@Aramui-MacBookPro wecode % git remote add origin https://github.com/aramcho206/wecode.git
    <!-- setting the git hub remote -->

aramcho@Aramui-MacBookPro wecode % git push origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 353 bytes | 176.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/aramcho206/wecode.git
 * [new branch]      main -> main

    <!--  pushed to github remote -->

aramcho@Aramui-MacBookPro wecode % git branch
* main
aramcho@Aramui-MacBookPro wecode % git branch feature/readme
aramcho@Aramui-MacBookPro wecode % git branch
  feature/readme
* main
aramcho@Aramui-MacBookPro wecode % git checkout feature/readme
M       test.js
Switched to branch 'feature/readme'
aramcho@Aramui-MacBookPro wecode % git branch
* feature/readme
  main
aramcho@Aramui-MacBookPro wecode % touch README.md
aramcho@Aramui-MacBookPro wecode % ls
README.md       test.js
aramcho@Aramui-MacBookPro wecode % 

