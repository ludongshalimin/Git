�����һ�δ����Javascript�����ύ��github�ϳ�����һЩ����
��github�ϴ����������󣬱���Ҳ�����˶�Ӧ���ļ��д����ȫ���������ύ��ȥ��
����û����ӳɹ�����ʾ error:src refspec master does not match any


������Լ��ķ������github�汾�������أ������������Ļ�����˾�Ķ����Ϳ��ԣ�������
 
 �����ļ���
 mkdir learngit
 �����ļ���
 cd learngit
 �����ļ�
 touch README


 ��Ŀ¼���GIt���Թ���Ĳֿ�
 git init

 //����git���ļ���ӵ��ֿ⣬ֻ��ӵ��ݴ��������Զ��add,һ��commit
 commit����ӵ��ǰ��ݴ��������������ύ����ǰ��֧
 git add readme.txt
 ���Զ��add һ���ύ
 git commit -m "message"


 �鿴�ֿ�ĵ�ǰ״̬
 git status

 �鿴�ļ��Ĳ�ͬ
 git diff readme.txt
 �鿴�ļ�������
 cat readme.txt

 �鿴�ύ��ʷ���Ա�ȷ��Ҫ�˻ص��ĸ�����
 git log --pretty=oneline


 �汾����
 HEAD:��ʾ��ǰ�汾
 HEAD ^:��ʾ��һ���汾
 HEAD ^^:��ʾ����һ���汾
 ���ص���һ���汾
 git reset --hard HEAD^
 �鿴�޸�������ʷ
 git reflog 


 �����޸�
 git checkout --readme.txt
 �����ǣ��ð汾��������ļ��滻�����������ļ����ļ�
 ��˼�ǣ���readme.txt�ļ��ڹ��������޸�ȫ���������������������
 		 һ���ǣ�readme.txt���޸�֮�󣬻�û�б��ŵ��ݴ��������ڳ����޸ľͻص��˺Ͱ汾��һģһ����״̬
 		 ��һ��,�Ѿ���ӵ��ݴ������������޸ģ����ڳ����ͻص���ӵ��ݴ������״̬
���������Ѿ�git add �ˣ����޸���ӵ��ݴ�����
�Ȱ��ݴ������޸����,����������
git reset HEAD readme.txt
Ȼ����չ�����
git checkout --readme.txt

����Ѿ����ļ��ύ���汾�������ˡ�����ǰ�İ汾����.����ǰ����û�����͵�Զ�̿�


�Ӱ汾����ɾ���ļ�
git add test.txt
git commit -m "add test.txt"
//��仰��ɾ���˱��ع��������ļ�test.txt.�����������Ͱ汾��������ļ��Ͳ�һ����
rm test.txt
//ɾ���汾�������test.txt
git rm test.txt
git commit -m "remove test.txt"
�����ɾ�˱��ص��ļ�������һ����ԭ,�ð汾������İ汾�滻�������İ汾
git checkout --test.txt


�Զ��github������
ssh-keygen -t rsa -C "youremail@example.com"
���û���Ŀ¼����.sshĿ¼������id_rsa��id_rsa.pub,һ��˽Կ��һ����Կ
��������Ŀ���Ǳ�֤���������ҵĵ���

����һ��Զ�̿�
����һ��Զ�̿�
git remote add origin git@github.com:ludongshalimin/javascriptlearn.git
������ʹ�����������һ������master��֧
git push -u origin master
�Ժ�ʹ������������µ��޸�
git push origin master


��¡Զ�̿⵽����
git clone git@github.com:ludongshalimin/javascriptlearn.git


��֧����
//�������л���dev��֧
git checkout -b dev
�൱��
git branch dev ; 
git checkout dev
git branch �г����еķ�֧
��֧�Ѿ��޸���ϣ�����Ҫ�л�������֧��
git checkout master
dev��֧��master��֧���кϲ�
git merge dev
git branch -d dev
��git �޷��Զ��ϲ���֧ʱ���ͱ������Ƚ����ͻ�������ͻ�����ύ���ϲ����
Ϊʲô���г�ͻ�����أ�1������֧���ڷ�֧�Ͻ������޸�Ȼ��������ύ
					  2�л�������֧��Ȼ������֧�Ͻ������޸ģ��ύ
					  3���кϲ������ֳ�ͻ
���������git status
		  ֱ�Ӳ忴�ļ������޸ģ�Ȼ��git add ;git commit -m "conflict fixed"
��git log --graph --pretty=online �鿴��֧�ϲ������

//no-ff����ʾ���� fast forward
git merge --no-ff -m "merge message"
��֧����
master��֧Ӧ���Ƿǳ��ȶ��ģ��������������°汾��ƽʱ����������ɻ�
�ɻ��dev��֧�ϣ�dev��֧�ǲ��ȶ���,
��ĳ��ʱ�򣬱���1.0�汾������ʱ���ٰ�dev��֧�ϲ���master
��С�����ÿ���˶���dev��֧����ɻ
ÿ���˶����Լ��ķ�֧��ʱ��ʱ����dev��֧�Ϻϲ��Ϳ���




����޸�bug
�޸�bugʱ�����ǻ�ͨ�������µ�bug��֧�����޸���Ȼ��ϲ������ɾ��
����ͷ����û����ɵ�ʱ���Ȱѹ����ֳ�git stashһ�£�Ȼ��ȥ�޸�bug
�޸�����git stash pop,�ص������ֳ�
Ҳ���Զ��git stash 
��git list�鿴
Ȼ�� git stash apply stash@{0};������һ�����е���


�¹���feature��֧
����һ���¹��ܣ�����½�һ����֧
���Ҫ����һ��û�б��ϲ����ķ�֧������ͨ�� git branch -d <name>����ǿ��ɾ��



����Э��
�鿴Զ�̿����Ϣ��ʹ��git remote -v
�ӱ������ͷ�֧��ʹ��git push origin branch-name 
�������ʧ�ܣ�����ΪԶ�̷�֧������ı��ظ��£�����git pullץȡԶ�̵����ύ
����ķ����ͷ�֧�����еĽ����ͻ�ķ�����ȫһ����
�ڱ��ش�����Զ�̷�֧��Ӧ�ģ�ʹ��git checkout -b brachname origin/branchname
�������ط�֧��Զ�̷�֧������
ʹ��git branch --set-upstream branchname origin/branchname


��ǩ����

tag������һ������������֣����磬v1.1����ĳ��commit����һ��
�Ե�ǰ�������ύ���ϱ�ǩ
git tag v1.0
//��ζ���ʷ���ύ�汾���ϱ�ǩ
�����ҵ���ʷ�İ汾
git log 

git tag v0.9 6224937
git push origin <tagname>��������һ�����ر�ǩ
git push origin --tags����ȫ��δ���͹��ı��ر�ǩ
git tag -d <tagname> ɾ��һ�����صı�ǩ


















