## subqueries!!!!

![alt text](image-12.png)

region for:
- each customer
    - who had an order with freight over 100



= 

all customer IDs for order with freight over 100
customer information (region)
combine


![alt text](image-13.png)

![alt text](image-14.png)

start from inner most 
(start from the most complex one)


query will process the inner most first as well

![alt text](image-15.png)



### subqueries for calculations

![alt text](image-16.png)
![alt text](image-17.png)


this is fine too 

![alt text](image-18.png)

![alt text](image-19.png)

![alt text](image-20.png)



给一个id，科目；成绩的表，搜索不及格科目大于两门课的学生id。


```sql
select id
from student_scores
where score<60
group by id
having count(*) > 2

```


