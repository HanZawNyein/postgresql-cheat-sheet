-- inner join, multiple joins
-- select partner_id,u.id,u.partner_id,login from res_users u join res_partner p on u.partner_id = p.id

-- self joins
-- select * from hr_employee join hr_employee as e on e.id = hr_employee.id;

-- left join 
-- table 1 left join table 2 only conditions record

-- outer joins
-- select * from hr_employee left join hr_employee as e on e.id = hr_employee.id;
-- select * from hr_employee right join hr_employee as e on e.id = hr_employee.id;

-- using clause
-- select s.partner_id,u.partner_id from sale_order s join res_users u on s.partner_id = u.partner_id;
-- select s.partner_id,u.partner_id from sale_order s join res_users u using(partner_id);

-- select s.partner_id,u.partner_id from sale_order s join res_users u on s.partner_id = u.partner_id and s.id =u.id;
-- select partner_id,u.id,u.partner_id,login from res_users u join res_partner p using(id,partner_id)

-- natural joins same column one join
-- natural joins column are always show in first
-- select * from sale_order natural join res_users;

-- cross joins
-- select res_users.id,res_users.partner_id,res_partner.id from res_users cross join res_partner;

-- union
-- select id,login,create_date from res_users  where create_date < '2023-07-03 06:45:49.670752' union
-- select id,login,create_date from res_users  where create_date > '2023-07-03 06:45:49.670752';
