�Ϳ������ Martus(tm) ��� readme_verify_th.txt
------------------------------------------------------------

Benetech ��Ѻ��ا����� Martus ���ҧ������ͧ
�ô��Ǩ�ͺ�����������ش���� http://www.martus.org ��л�ԺѵԵ�����йӷ��
��ҡ������䫵�㹡�ô�����Ŵ�Ϳ������������ ���������  SHA-1 sum 

�͹Ҥ� Benetech �Ҩ���͡����ᨡ������蹻�Ѻ��ا�ͧ��� martus.jar �س�����
�������� martus.jar � � ���������س �����Ҥس�����Ǩ�ͺ��������繢ͧ
��ԧ ���������㨢�鹵͹��õ�Ǩ�ͺ��� � ��觨з����س���㨼Դ��

�����������Ǩ�ͺ��辺���մ� Martus ������Ѻ����׹�ѹ������ҹ��
����ǹ�������Ǣ����� "Verifying a Martus jar file" ��˹�Ҵ�ǹ���Ŵ Martus ����Ѻ
���й�㹡�õ�Ǩ�ͺ�Ϳ������ Martus ���йӴѧ���� ���������������Ǩ�ͺ�����
������ Verify 㹫մ� Martus ��Ҥس���������Ǩ�ͺ���躹�蹴�ʡ����ͺ�
���촴�ʡ� �س��ͧ����¹���й�����ʹ���ͧ�Ѻ���س��


* ��Թ���� (Windows):

�Դ˹�ҵ�ҧ�ͧ MS-DOS ���Ǿ�������� 3 ��÷Ѵ���ŧ� ᷹�����쿫մ�����ͧ�س
�ҡ "d" ���ǾҸ�ͧ��� .jar ���س��ͧ��õ�Ǩ�ͺ

d:
cd  \verify
ven  c:\path-to-file\martus.jar

���ͨҡ Start menu ���͡ Run ���Ǿ����:

d:\verify\ven  c:\path-to-file\martus.jar  

(����� d �����쿫մ�����ͧ�س ��� path-to-file ��;Ҹ�ͧ��� .jar ���س��ͧ���
��Ǩ�ͺ)

��һ�ҡ� "Martus JAR verified." �ʴ������� .jar ��鹶١��ͧ


* ��������� (Mac):

�ҧ��� .jar ����ŧ������� Martus ����������Ǻ����촴�ʡ�ͧ�س �����ѹ
���������ͺ:

cd  /Volumes
ls
cd  Martus (�ҡ��鹡�����᷺ ��������������������ѵ��ѵ�)
cd  verify
java  -cp  .  JarVerifier  /Library/Java/Martus/martus.jar

��һ�ҡ� "Martus JAR verified." �ʴ������� .jar ��鹶١��ͧ



* ��Թء�� (Linux):

�ҧ��� .jar ����ŧ������� ~/.Martus/ ������������� �����ѹ��ǵ�Ǩ�ͺ
�鴵��������ö�ҧ� bash ���� sh ������ (�����Ҥس��ͧ�� 'root' 㹢�з��
��ͧ������ mount):

  mount=/mnt/cdrom
  [ -d $mount ] || mount=/cdrom		# for Debian and etc
  [ -d $mount/[vV]erify ] || mount -r $mount
  cd $mount/[vV]erify && java JarVerifier ~/.Martus/martus.jar

��һ�ҡ� "Martus JAR verified." �ʴ������� .jar ��鹶١��ͧ

��Ҥس��� � bash: java: No such file or directory� �ʴ���Ҥس��ͧ����������
bin �ͧ Java ŧ� PATH �ͧ�س
�٢�鹵͹��� 1 㹢�鹵͹��õԴ��駺��Թء��

��Ҥس��� �Error loading class JarVerifier: Bad major version number� �ʴ����
�س��ͧ�Դ��� Java ���������� ���/���� ���Ҹ�ͧ Java ����������شŧ�
PATH �ͧ�س �٢�鹵͹��� 1 㹢�鹵͹��õԴ��駺��Թء��
