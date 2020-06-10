1. new work;
2. add two;
3. add three;

4. git push origin branchname// 在远程创建同名分支
5. already up to date的报错的处理：
git checkout master
git reset --hard 分知名
git push --force origin master
//

6.第五条无效，在远程修改后，在本地重新git pull

4.
/*
在本地进行开发结束后，使用 Git branch -d branchName 删除本地分支。
此时如果想同步删除已经 Merge 到 Master 的远程分支，使用 git push origin --delete branchName 进行删除。
*/

5.
/*
如果本地新建了一个分支 branch_name，但是在远程没有。
这时候 push 和 pull 指令就无法确定该跟踪谁，一般来说我们都会使其跟踪远程同名分支，
所以可以利用 git push --set-upstream origin branch_name ，这样就可以自动在远程创建一个 branch_name 分支，
然后本地分支会 track 该分支
*/
git push --set-upstream origin branch_name


