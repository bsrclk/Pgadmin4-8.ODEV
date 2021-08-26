# Pgadmin4-8.ODEV
8.ÖDEV
create table employee
(id serial primary key,
 name VARCHAR(50),
 birthday DATE,
 email VARCHAR(100)
);


select count(*) from employee

update employee
set name='LUZZZ',
 birthday='1999-05-10',
 email='rngjkrngkjntrkg'
 where id=2;


update employee
set name='pamuk',
 birthday='1950-05-10',
 email='prpepepepepep'
where name ILIKE 'A%'
returning * ;

update employee
set name='POYRAZ'
WHERE id between 3 and 6
returning * ;


update employee
set email ='rnjrnıgnıtngntr'
WHERE id in (8,9,10) and email ILIKE 'o%'
returning * ;



delete from employee
where id=5

delete from employee
where email like 'a%'


delete from employee
where id between 3 and 5 
