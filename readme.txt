1) create file readme.me
2) create file sensitive_data. This file by "mistake" was including in the repo, but shouldn't cuz there are password and stuff I shouldn't share
3) naively delete the file "sensitive_data" and commit
  git rm [file]
  git commit
3.1) anyone can see the previous commit (step 2) and see the info.
4) Use "bfg" to remove de file from git (rewrite history)
  java -jar bfg.jar --delete-files [file]
