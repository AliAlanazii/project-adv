# project-adv
#### Q1: Count Total Cinema Halls
```sql
SELECT COUNT(*) AS total_cinema_halls FROM KSA;
```
<img width="1061" alt="Screenshot 1446-08-12 at 8 59 44 PM" src="https://github.com/user-attachments/assets/19cea955-b675-4590-bd74-b0800f9552ef" />

#### Q2: Top 5 Highest-Rated Cinema Halls
```sql
SELECT name, rating FROM KSA ORDER BY rating DESC LIMIT 5;
```
<img width="1061" alt="Screenshot 1446-08-12 at 9 13 33 PM" src="https://github.com/user-attachments/assets/94b1dccc-81cb-4c70-a48b-6c7f39ceb063" />


#### Q3: Average Rating of All Cinema Halls
```sql
SELECT AVG(rating) AS average_rating FROM KSA;
```
<img width="1061" alt="Screenshot 1446-08-12 at 9 13 59 PM" src="https://github.com/user-attachments/assets/64d4ff1c-5b35-4eb9-ab35-0614d2c931c4" />

#### -- Q4: review every thing inside Riyadh my city!!!
```sql
SELECT * FROM KSA WHERE location = 'Riyadh';
```
<img width="1061" alt="Screenshot 1446-08-12 at 9 17 11 PM" src="https://github.com/user-attachments/assets/d8eefff3-db20-491f-8511-2b07b96903b0" />

#### Q5: Count Cinema Halls with Rating < 3
```sql
SELECT COUNT(*) AS low_rated_halls FROM KSA WHERE rating < 3;
```
<img width="1061" alt="Screenshot 1446-08-12 at 9 17 53 PM" src="https://github.com/user-attachments/assets/8f60b43b-e22c-4d1d-98c6-9eb2e32ab87c" />

#### Q6: Find cinemas with the word 'Mall' in their name
```sql
SELECT name, location FROM KSA WHERE name LIKE '%Mall%';
```
<img width="1061" alt="Screenshot 1446-08-12 at 9 22 28 PM" src="https://github.com/user-attachments/assets/64f4021e-da0d-4210-a44d-75392412a0ec" />

#### Q7: Group Cinema Halls by Location
```sql
SELECT location, COUNT(*) AS hall_count FROM KSA GROUP BY location;
```
<img width="1061" alt="Screenshot 1446-08-12 at 9 23 10 PM" src="https://github.com/user-attachments/assets/421f7732-5889-44a8-af1f-6829e0c48517" />

#### Q8: Lowest-Rated Cinema Hall
```sql
SELECT name, rating FROM KSA ORDER BY rating ASC LIMIT 1;
```
<img width="1061" alt="Screenshot 1446-08-12 at 9 24 34 PM" src="https://github.com/user-attachments/assets/696a984b-552a-4bca-af53-5d96ae899e5f" />
#### Q9: Cinema Halls with "Amazing" in Comments
```sql
SELECT * FROM KSA WHERE LOWER(comments) LIKE '%amazing%';
```
<img width="1061" alt="Screenshot 1446-08-12 at 9 28 46 PM" src="https://github.com/user-attachments/assets/04f7f897-5baa-4707-bfc8-1fce2e23ee6d" />


#### Q 10: Cinema Halls with Ratings Between 4 and 5
```sql
SELECT * FROM KSA WHERE rating BETWEEN 4 AND 5 ORDER BY location;
```
<img width="1061" alt="Screenshot 1446-08-12 at 9 29 41 PM" src="https://github.com/user-attachments/assets/809cb4df-b6dd-4d65-afcb-8f01b15040b4" />










