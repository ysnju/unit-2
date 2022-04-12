
--query the database to know waht is inside
select * from person limit 1;
--find all names starting with c
select name, id from person where name like 'Alexis%';
select count(name) from person where name like 'A%';
select name,id from person where name like 'Alexis%';
select annual_income from income where ssn =651475435;

--find highest income
select ssn, annual_income from income order by annual_income desc limit 4;
select count(annual_income) from income where annual_income > 35000;
select count(annual_income) from income where annual_income < 35000;

select * from crime_scene_report;
--what is the city with more reports typed murder（できない）
select city from crime_scene_report where type like 'murder';
--'how many people drive Mercedez-Benz'(353)
select count(car_make) from drivers_license where car_make like 'Mercedes-Benz';
--'what is the frequency（？） of people living in the same street'（できない）

--how many report for theft in SQL city(9)
select count(type like 'theft') from crime_scene_report where city like 'SQL city';
--how many events happened on facebook during July 2017 (1213)
select count(event_id) from facebook_event_checkin where date like '201706%';
--the range of the annual income for individual with gold membership(できない)
select person_id from get_fit_now_member where membership_status like 'gold';
--how many crimes happened at night(3)
select count(description) from crime_scene_report where description like '%night%';
--what month has the most number of crimes (June)
select count(description) from crime_scene_report where date like '201701%';
--86
select count(description) from crime_scene_report where date like '201702%';
--72
select count(description) from crime_scene_report where date like '201703%';
--78
select count(description) from crime_scene_report where date like '201704%';
--79
select count(description) from crime_scene_report where date like '201705%';
--73
select count(description) from crime_scene_report where date like '201706%';
--89
select count(description) from crime_scene_report where date like '201707%';
--67
select count(description) from crime_scene_report where date like '201708%';
--60
select count(description) from crime_scene_report where date like '201709%';
--85
select count(description) from crime_scene_report where date like '201710%';
--75
select count(description) from crime_scene_report where date like '201711%';
--88
select count(description) from crime_scene_report where date like '201712%';
--71
--how many crimes involved nudism(0)
select count(description) from crime_scene_report where description like '%nudism%';

--SQL murder
select id from drivers_license where plate_number like 'H42W';
Insert into solution values (1,'Jeremy Bowers');

Select value from solution;

select person_id from facebook_event_checkin where event_name like'%SQL Symphony concert%' and date like '201712%';
Insert into solution values (1,'Miranda Priestly');
Select value from solution

