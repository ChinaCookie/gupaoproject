Git�ύ�����Զ�ֿ̲� ���Ѿ�ϰ��ʹ��gitͬ��д���룬github����������й�ƽ̨�����ǹ������ڡ��㶮�ġ�ԭ���ٶȺ�������ʱ�޷����ʣ���������Լ��Ĵ���ͬ���������ͬ��Զ�ֿ̲ⱸ�ݡ�

�ҵ���Ҫ�ֿ�:
[github] https://github.com/wonux/test.git ���ֿ�
[oschina] https://git.oschina.net/wonux/test.git ���ڳ��òֿ�

���⣬���ڻ���coding(ԭ����gitcafe�ϲ�����coding),csdn code�ȡ�

���ͬ����Զ�ֿ̲�
���һ��remote,������all,Ҳ�����Ǳ������(��origin)

git remote add all https://github.com/wonux.test.git�������һ��:

git remote set-url --add all https://git.oschina.net/wonux/test.git�ظ���ͬһ��Զ�ֿ̲����������Ҫset-url --add����

����ж��,����������һ������������.

���Զ�ֿ̲����ʹ���
git push all --all�����ͻ�һ���ύ���������,���������������:

git push all --all
Username for 'https://github.com': wonux
Password for 'https://wonux@github.com': 
Counting objects: 68, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (56/56), done.
Writing objects: 100% (68/68), 72.16 KiB | 0 bytes/s, done.
Total 68 (delta 13), reused 0 (delta 0)
To https://github.com/wonux/test.git
 * [new branch]      master -> master
Username for 'https://git.oschina.net': wonux
Password for 'https://wonux@git.oschina.net': 
Counting objects: 68, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (56/56), done.
Writing objects: 100% (68/68), 72.16 KiB | 0 bytes/s, done.
Total 68 (delta 13), reused 0 (delta 0)
To https://git.oschina.net/wonux/test.git
 * [new branch]      master -> master��ס��Ҫ����--all�������������--all�����޷����ͣ���ʾ��

git push all
warning: push.default is unset; its implicit value has changed in
Git 2.0 from 'matching' to 'simple'. To squelch this message
and maintain the traditional behavior, use:

  git config --global push.default matching

To squelch this message and adopt the new behavior now, use:

  git config --global push.default simple

When push.default is set to 'matching', git will push local branches
to the remote branches that already exist with the same name.

Since Git 2.0, Git defaults to the more conservative 'simple'
behavior, which only pushes the current branch to the corresponding
remote branch that 'git pull' uses to update the current branch.

See 'git help config' and search for 'push.default' for further information.
(the 'simple' mode was introduced in Git 1.7.11. Use the similar mode
'current' instead of 'simple' if you sometimes use older versions of Git)

fatal: unable to access 'https://github.com/wonux/test.git/': Couldn't resolve host 'github.com'���������ļ�
�ڲ������������������������Ǵ�.git/config�ļ�,���ǿ��Կ�������������:

[remote "all"]
    url = https://github.com/wonux/test.git
    fetch = +refs/heads/*:refs/remotes/all/*
    url = https://git.oschina.net/wonux/test.git��ˣ�ֱ����.git/config�ļ�����ӣ�

[remote "all"]
    url = https://github.com/wonux/test.git
    fetch = +refs/heads/*:refs/remotes/all/*
    url = �����ж��ٸ�Զ�̿�,�����ö��ٸ�url����.
��������Կ���,��һ�ַ������ɵ������л���һ��fetch����,������ÿ�����ȫȥ��.
