#create table client(
         client_id       NUMBER(5) PRIMARY KEY,
         client_name      VARCHAR2(15) NOT NULL,
         client_surname varchar(15) not null)

INSERT INTO client values (12345, 'Justyna', 'Misior')
insert into client values (12346, 'Jan', 'Kowalski')
insert into client values (12347, 'Adam', 'Nowak')
         
create table books(
        book_id NUMBER(5) PRIMARY KEY,
        title varchar2(40),
        author_name varchar2(15) NOT null,
        availability number(1,0))
        drop table books
        select * from books
insert into books values(12346, 'Harry Potter and the Philosophers Stone', 'Rowling', 1)
insert into books values(12342, 'Harry Potter and the Chamber of Secrets', 'Rowling', 1)
insert into books values(12343, 'Harry Potter and the Prisoner of Azkaban', 'Rowling', 1)
insert into books values(12345, 'Harry Potter and the Half-Blood Prince', 'Rowling', 1)
        
create table orders(
        order_id number(5),
        client_id number(5) constraint client_fkey REFERENCES client(client_id),
        book_id number(5) CONSTRAINT book_fkey REFERENCES books (book_id))
        
 "SELECT book_id, title, author_name, availability  FROM northwind.dbo.books       
        
        create table products(
        productid number(5) primary key, 
        productname varchar2(20))
        
        insert into products values (22345, 'ttt')
        select * from products
        
    

