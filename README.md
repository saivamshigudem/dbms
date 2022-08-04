# dbms
FIND THE Nth HIGHEST SALARY?
select distinct(sal) from emp order by sal desc limit n,1;
DISPLAY UNIQUE JOBS FROM EMP?
select distinct(jobs) from emp;
LIST THE DETAILS OF EMP IN ASCENDING ORDER OF THEIR DEPTNO AND DESCENDING ORDER OF JOBS?
select ename,deptno,job from emp order by  deptno, job desc;
LIST THE EMPNO,ENAME,SAL AND DAILY SAL OF ALL EMPLOYEE IN ASC ORDER OF THEIR DAILYSAL;
select ename,empno,sal/30 as dalsal from emp order by sal desc;
LIST THE ENAME WHO ARE EITHER CLAERK OR ANALYST IN DESC ORDER?
select ename,job from emp where job like 'clerk' or job like 'analyst' order by job;
LIST THE EMPNO,ENAME,SAL AND ANNUALSAL AND DESC ORDER BY ANNUALSAL?
select ename,empno,sal*12 as annualsal from emp order by sal*12 desc;
LIST THE ENAME THOSE ARE STARTING WITH S WITH 5 CHARACTERS?
select ename from emp where ename like 's%' and length(ename)=5;
LIST THE EMPLOYEES WORKING IN DEPATMENT 10 OR 20 IN DESCENDING ORDER?
select ename,deptno from emp where deptno='10' or deptno='20'order by deptno desc;
LIST THE NAME WHOSE NAMES HAS A SET OF LL TOGETHER?
select ename from emp where ename like '%ll%';
LIST THE EMPLOYEES WHO JOINED IN THE YEAR MONTH OF DECEMBER?
select ename,hiredate from emp where hiredate like '%-12-%';
LIST THE EMPLOYEES ANNUALSAL WHOSE IN BETWEEN 22000 TO 45000?
select ename,sal*12 as annaulsal from emp where sal*12 between 22000 and 45000;
