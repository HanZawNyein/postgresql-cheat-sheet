# postgresql-cheat-sheet

-- select login,id from res_users;
-- select login,id from res_users where login='admin';
-- select * from res_users order by login;
-- select * from res_users order by login desc;
-- select login,id from res_users order by 2,1 asc;

-- select login,id from res_users where id=2 order by login;
-- select login,id,id*2 as double from res_users where id=2 order by login;
-- select login,id,id*2 as double from res_users where id=2 order by login;
-- select login,partner_id,id,partner_id*2 as promotion from res_users where id=2 order by login;
-- select login,partner_id,id,partner_id*2 as "promotion pirce" from res_users where id=2 order by login;
-- select distinct active,id from res_users;

-- select login,id from res_users where id != 2;
-- select login,id from res_users where id <> 2;

-- select create_date from res_users where create_date <= '2022-11-01' and id >= 100;
-- select * from res_users where id in (1,2,3,5);
-- select * from res_users where id not in (1,2,3,5);
-- select * from res_users where id between 1 and 10;

-- select * from res_users where login like '%a';
-- select * from res_users where login not like '%a';
-- select * from res_users where login like 'a%';
-- select * from res_users where login like '%a%';

-- select * from res_users where login like '____n';
-- select * from res_users where login like 'a___n';

-- ERROR this regexp replace with ~
-- select name from res_partner where name  regexp  'Saw';

-- select name from res_partner where name like '%Saw%';
-- select name from res_partner where name ~ 'Saw';
-- select name from res_partner where name ~ 'Saw|U';

-- start word
-- select name from res_partner where name ~ '^Saw';

-- end word
-- select name from res_partner where name ~ 'Ah$';

-- select name from res_partner where name ~ 'e[y,ies]';
-- select name from res_partner where name ~ '[a-e]e';

-- select name,company_id from res_partner where company_id is not null;


-- select * from res_users limit 3;
