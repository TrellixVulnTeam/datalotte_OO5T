------------------------------README-------------------------------

*** �����͸� Ȱ���� �Һ��� �ൿ����

- ������ ������ ����, ���� �ݺ��н��� ���� �� �� ��Ȯ�� ������ �������� ��õ ���� ���� ����
- ������ ������ ���񽺸� �����ÿ� Ȱ���Ͽ� �� ������ �� ���� ����ȿ�� ���

- �м������ logistic regression, MLP classifier, DNN classifier
- ��Ȯ���� ���� ���� MLP ä��



*** ����Ʈ ���� ���

1. node.js ���� ����ּ��� lts��.... 
2. cmdâ���� �������� npm install �Ͻð� 
3. npm install -g yarn  �Ѵ���... 
4. �츮�� ������Ʈ�� �������� Ǭ��..  (��� C:\work\frontend ) , 
5. ��Ŭ�������� open project from .... �ؼ� C:\work\backend �������ų� �ű�� ����! 
6. cmd â���� activate test�Ѵ����� 

7. pip install djangorestframework �ϰ� 

create database project2 
use project2 


mysql���� ���̺��� ������ּ��� 
	1. Product table
create table product (
   CLNT_ID int(50),
   SESS_ID int(50),
   HITS_SEQ int(50),
   PD_C int(50),
   PD_ADD_NM varchar(50),
   PD_BRA_NM varchar(50),
   PD_BUY_AM  int(50) ,
   PD_BUY_CT int(50),
   result int(50)
)charset=utf8;

LOAD DATA LOCAL INFILE "C:/work/danal/lotte/product_sample.csv" INTO  TABLE project2.product FIELDS TERMINATED BY "," IGNORE 1 LINES;
	2. Customcreate table custom (
	CLNT_ID int(50),
	CLNT_GENDER varchar(10),
	CLNT_AGE int(10))charset=utf8;LOAD DATA LOCAL INFILE "C:/work/danal/lotte/custom_sample.csv" INTO  TABLE project2.custom FIELDS TERMINATED BY "," IGNORE 1 LINES;
	3. Masterdrop table master;create table master (PD_C int(50),
	PD_NM varchar(50),
	CLAC1_NM varchar(50),CLAC2_NM varchar(50),CLAC3_NM varchar (50)
	)charset=utf8;LOAD DATA LOCAL INFILE "C:/work/danal/lotte/master_2.csv" INTO  TABLE project2.master FIELDS TERMINATED BY "," IGNORE 1 LINES;
	4. Session
	CLNT_ID    SESS_ID   SESS_SEQ  SESS_DT     TOT_PAG_VIEW_CT TOT_SESS_HR_V  DVC_CTG_NM ZON_NM       CITY_NM   day
	1124907    8942818   1         2018-05-04  18              1917           desktop    Gyeonggi-do  Ansan-si  Friday
	create table session (
	CLNT_ID varchar(50),
	SESS_ID varchar(50),
	SESS_SEQ int(30),
	SESS_DT date,
	TOT_PAG_VIEW_CT int(30),
	TOT_SESS_HR_V int(30),
	DVC_CTG_NM varchar(50),
	ZON_NM varchar(50),
	CITY_NM varchar(50),
	day varchar(20)
	)charset=utf8LOAD DATA LOCAL INFILE "C:/work/danal/lotte/session_sample.csv" INTO  TABLE project2.session FIELDS TERMINATED BY "," IGNORE 1 LINES




8. ��� run server ���ּ���  localhost:8000 �� ���� �ߴ��� Ȯ��! 
8. �ٸ� cmd â���� cd C:\work\frontend �ϰ� 
9. �� ��ο��� yarn start  �ϸ� ¥�� !  localhost:3000  �� �ߴ��� Ȯ��! 



