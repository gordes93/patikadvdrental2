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

