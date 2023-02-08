# SQL-Odev8
## UPDATE-DELETE Yapısı

1) test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.

CREATE TABLE employee (
    id SERIAL PRIMARY KEY,
    name VARCHAR(50),
     birthday DATE,
     email VARCHAR(100)
);

2) Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.

insert into employee (name, birthday, email) values ('Kevan', '1933-08-16', 'kgranham0@facebook.com');
insert into employee (name, birthday, email) values ('Sally', '1961-08-10', 'salcalde1@behance.net');
insert into employee (name, birthday, email) values ('Ivor', '1915-03-27', 'imanson2@sciencedirect.com');
insert into employee (name, birthday, email) values ('Abramo', '1949-11-29', 'ablunderfield3@reddit.com');
insert into employee (name, birthday, email) values ('Mannie', '1940-09-06', 'mturbern4@narod.ru');
insert into employee (name, birthday, email) values ('Raddy', '1952-06-28', 'rwiddison5@businessinsider.com');
insert into employee (name, birthday, email) values ('Georgina', '1910-03-14', 'gbiaggioni6@amazon.co.jp');
insert into employee (name, birthday, email) values ('Tanya', '1903-05-27', 'tviel7@vistaprint.com');
insert into employee (name, birthday, email) values ('Wilfrid', '1904-07-30', 'wkilleley8@latimes.com');
insert into employee (name, birthday, email) values ('Opaline', '1907-09-06', 'ocoffee9@imageshack.us');
insert into employee (name, birthday, email) values ('Blancha', '1947-03-08', 'bmingeta@cargocollective.com');
insert into employee (name, birthday, email) values ('Barty', '1963-12-03', 'bcovottib@abc.net.au');
insert into employee (name, birthday, email) values ('Jodi', '1991-07-22', 'jmacfallc@webmd.com');
insert into employee (name, birthday, email) values ('Turner', '1924-07-05', 'tcorderoyd@cmu.edu');
insert into employee (name, birthday, email) values ('Costa', '1953-03-11', 'clethabridgee@goodreads.com');
insert into employee (name, birthday, email) values ('Haleigh', '1930-12-24', 'hfradgleyf@upenn.edu');
insert into employee (name, birthday, email) values ('Orly', '1954-05-20', 'osickamoreg@umn.edu');
insert into employee (name, birthday, email) values ('Neils', '1964-01-08', 'neasemanh@timesonline.co.uk');
insert into employee (name, birthday, email) values ('Lydon', '1907-08-14', 'lmackneyi@amazon.co.jp');
insert into employee (name, birthday, email) values ('Carly', '1941-10-05', 'cshinfieldj@shareasale.com');
insert into employee (name, birthday, email) values ('Marigold', '1955-06-17', 'mtregienk@webeden.co.uk');
insert into employee (name, birthday, email) values ('Dallon', '1952-11-07', 'dquenel@squarespace.com');
insert into employee (name, birthday, email) values ('Salomi', '1975-08-09', 'sbollardm@apple.com');
insert into employee (name, birthday, email) values ('Delbert', '1905-12-09', 'dcarnn@hexun.com');
insert into employee (name, birthday, email) values ('Hilly', '1965-10-10', 'hchellamo@plala.or.jp');
insert into employee (name, birthday, email) values ('Ferdie', '1955-08-06', 'fprattyp@symantec.com');
insert into employee (name, birthday, email) values ('Llewellyn', '1959-01-29', 'loxtobyq@a8.net');
insert into employee (name, birthday, email) values ('Hatti', '1952-10-11', 'harnautr@liveinternet.ru');
insert into employee (name, birthday, email) values ('Jannel', '1941-06-07', 'jdewiss@ustream.tv');
insert into employee (name, birthday, email) values ('Kimberli', '1938-12-22', 'kharlowt@meetup.com');
insert into employee (name, birthday, email) values ('Tabbie', '1985-09-28', 'tdrainsu@senate.gov');
insert into employee (name, birthday, email) values ('Regen', '1970-02-22', 'rdeev@ca.gov');
insert into employee (name, birthday, email) values ('Lyndy', '1969-05-30', 'lphilbrookw@huffingtonpost.com');
insert into employee (name, birthday, email) values ('Clarisse', '1923-12-11', 'ckobierax@archive.org');
insert into employee (name, birthday, email) values ('Nyssa', '1962-12-21', 'nfranciottiy@deviantart.com');
insert into employee (name, birthday, email) values ('Maggi', '1977-11-06', 'mdrewz@devhub.com');
insert into employee (name, birthday, email) values ('Katrine', '1942-01-25', 'ksivyour10@cisco.com');
insert into employee (name, birthday, email) values ('Dorris', '1927-02-16', 'dgallone11@ning.com');
insert into employee (name, birthday, email) values ('Hildegarde', '1941-12-08', 'hhutchison12@oracle.com');
insert into employee (name, birthday, email) values ('Jonis', '1988-01-10', 'jpinks13@prlog.org');
insert into employee (name, birthday, email) values ('Pammie', '1980-11-15', 'pbuttner14@blinklist.com');
insert into employee (name, birthday, email) values ('Isiahi', '1907-05-16', 'iaucoate15@nps.gov');
insert into employee (name, birthday, email) values ('Lanni', '1934-05-28', 'losiaghail16@vinaora.com');
insert into employee (name, birthday, email) values ('Holden', '1972-01-01', 'hkobu17@trellian.com');
insert into employee (name, birthday, email) values ('Annabel', '1928-02-07', 'ahertwell18@rediff.com');
insert into employee (name, birthday, email) values ('Alane', '1949-08-26', 'amcilvaney19@issuu.com');
insert into employee (name, birthday, email) values ('Byran', '1976-02-15', 'bgreet1a@nifty.com');
insert into employee (name, birthday, email) values ('Casandra', '1939-10-19', 'cfeldmus1b@msn.com');
insert into employee (name, birthday, email) values ('Blinni', '1923-01-20', 'bturnbull1c@addthis.com');
insert into employee (name, birthday, email) values ('Drusie', '1936-12-24', 'dscurrey1d@cloudflare.com');


3) Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.

UPDATE employee
SET name = 'Wayne',
WHERE id = 3,
RETURNING *;

UPDATE employee
SET birtday = '1939-10-03',
WHERE birtday = '1939-10-19,
RETURNING *;

UPDATE employee
SET name = 'Eric',
    email = 'eric@rangh.com,
WHERE name = 'Casandra,
RETURNING *;

UPDATE employee
SET name = 'Abcd',
WHERE id > 48 
RETURNING *;

UPDATE employee
SET email = 'abcd@dcba.com',
WHERE name LIKE 'A%' 
RETURNING *;

4) Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.

DELETE FROM employee
WHERE id = 1
RETURNING *;

DELETE FROM employee
WHERE name = 'Abcd'
RETURNING *;

DELETE FROM employee
WHERE name LIKE 'A%'
RETURNING *;

DELETE FROM employee
WHERE email = 'abcd@dcba.com'
RETURNING *;

DELETE FROM employee
WHERE id > 18
RETURNING *;
