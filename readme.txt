Git is a version control system.
Git is free software.

��һ����������git add����Git�����ļ���ӵ��ֿ⣺
git add readme.txt
git add file2.txt file3.txt
����һ����Ӷ���ļ�
�ڶ�����������git commit����Git�����ļ��ύ���ֿ⣺
git commit -m "wrote a readme file"
�򵥽���һ��git commit���-m����������Ǳ����ύ��˵��

git status�������������ʱ�����ղֿ⵱ǰ��״̬
git diff readme.txt �鿴�ļ������޸���ʲô����

git log �鿴�ύ��־
git log --pretty=oneline �鿴�ύ��־���򻯰�

git reset --hard HEAD^ ���˵���һ���汾����һ���汾����HEAD^������һ���汾����HEAD^^����Ȼ����100���汾д100��^�Ƚ�������������������д��HEAD~100��
git reflog ������¼���ÿһ������


�޸����ļ� git addֻ��ѵ�ǰ���޸���ӵ��ݴ�����֮���޸ĵ�ÿ���޸Ķ�Ҫgit add��git commit�Ż��ύÿ���޸ĵ� 

git checkout -- readme.txt��˼���ǣ���readme.txt�ļ��ڹ��������޸�ȫ�����������������������

һ����readme.txt���޸ĺ�û�б��ŵ��ݴ��������ڣ������޸ľͻص��Ͱ汾��һģһ����״̬��

һ����readme.txt�Ѿ���ӵ��ݴ������������޸ģ����ڣ������޸ľͻص���ӵ��ݴ������״̬��

��֮������������ļ��ص����һ��git commit��git addʱ��״̬��


git rm readme.txt����ɾ��һ���ļ������һ���ļ��Ѿ����ύ���汾�⣬��ô����Զ���õ�����ɾ������ҪС�ģ���ֻ�� git checkout -- readme.txt �ָ��ļ������°汾����ᶪʧ���һ���ύ�����޸ĵ����ݡ�


Creating a new branch is quick.