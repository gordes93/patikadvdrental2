# patikadvdrental2
--select * from film where replacement_cost between 12.99 and 16.99
--select first_name, last_name from actor where first_name in ( 'Penelope', 'Nick', 'Ed')
--select * from film
--where rental_rate in ( 0.99, 2.99, 4.99) and replacement_cost in ( 12.99, 15.99 , 28.99)
# patikadvdrental3
--select * from country where country like 'A%a'
--select * from country where country like '_____%n'
--select title from film where title ilike '%T%T%T%T%'
--select * from film where (title like 'C%') and length > 90 and rental_rate = 2.99
# patikadvdrental4
--select distinct replacement_cost from film
--select count(distinct replacement_cost) from film
--select count(title) from film where (title like 'T%') and rating = 'G'
--select count(country) from country where country like '_____'
--select count(city) from city where city like 'R%' or city like '%r'
# patikadvdrental5
--select title from film where title like '%n' order by length desc limit 5
--select title from film where title like '%n' order by length asc limit 5 offset 5 
--select * from customer where store_id = 1 order by last_name desc limit 4
# patikadvdrental6
--select round(avg(rental_rate),3) from film
--select count(title) from film where title like 'C%'
--select max(length) from film where rental_rate = 0.99
--select count(distinct replacement_cost) from film where length > 150
# patikadvdrental7
--select rating,count(*) from film group by rating
--select replacement_cost, count(title) from film group by replacement_cost 
--having count(title) > 50
--select store_id, count(customer) from customer group by store_id
--select country_id, count(city) from city group by country_id order by count(city) desc limit 1
# patikadvdrental8
-- create table employee(
-- 	id serial primary key,
-- 	name varchar(50),
-- 	birthday Date,
-- 	email varchar(50)
-- )
--update employee set name = 'Ahmet' where name = 'Latrena'
--update employee set birthday = '1982-05-18' where name = 'Giustino' and birthday = '1926-06-20'
--update employee set email = 'fracier@marriott.com' where name = 'Frasier' and email = 'fsicelya@marriott.com'
--update employee set name = 'Mehmet' where name = 'Nanon'
--update employee set name = 'Ayşe' where name = 'Frannie'
--delete from employee where name = 'Ahmet'
--delete from employee where name = 'Mehmet'
--delete from employee where id = 8
--delete from employee where birthday = '1979-05-03'
--delete from employee where email = 'fvannonil@cornell.edu'
# patikadvdrental9
--select city,country from city inner join country on city.country_id = country.country_id
--select payment_id, first_name, last_name from customer inner join payment on payment.customer_id = customer.customer_id
--select rental_id, first_name, last_name from customer inner join rental on customer.customer_id = rental.customer_id
# patikadvdrental10
--select city, country from city left join country on city.country_id = country.country_id
--select first_name, last_name, payment_id from customer right join payment on customer.customer_id = payment.customer_id
--select first_name, last_name, rental_id from customer full join rental on customer.customer_id = rental.customer_id
