
## SQL Tips

```sql
distinct works for all columns;
limit 5 offset 6 (jump start from line 7 )
-- this is the comments 
/* Common comment format for
   different language */
order by c1 desc, c2; --asc is the default
order by 1,2; -- this also works
the A and a is the same within the dictionary, so it works in DBMS, the admin can change it

<> != !> ;between x and y; is null;
where A or B and C; -- the and will be do first, the sql running like (A and C), then (or B)
where (A or B) and C;
where vendid IN ("A","B") -- same logic like or, and the IN clause can include the "Select xxxx" and run faster
where NOT A; -- like <> and we can use the NOT IN (Select )
LIKE "Fish%" -- start from Fish % can not match the NUL, % can be 0 wildcard. in access, _ _ match with the single byte
-- % make the SQL query works slow, limit the useage of the %
Select RTRIM(A) + '(' + RTRIM(B) + ')' -- use the RTRIM to delete the right side spaces of the values
trim(), ltrim(), rtrim()
Select RTRIM(A) + '(' + RTRIM(B) + ')' 
AS C -- C could be the alias of the new column in SQL, if the column name is illegal, use the alias 
select Now() -- return you the current date and time
```
