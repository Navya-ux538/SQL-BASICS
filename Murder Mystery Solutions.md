1.
SELECT * 
FROM crime_scene_report;

2.
SELECT *
FROM crime_scene_report
WHERE type = "murder";

3.
SELECT *
FROM crime_scene_report
WHERE type = "murder"
  AND date = "20180115"
  AND city = "SQL City";

4.
SELECT *
FROM person;

5.
SELECT *
FROM person
WHERE address_street_name = "Northwestern Dr"
ORDER BY address_number DESC;

6.
SELECT *
FROM person
WHERE name LIKE '%Annabel%'
  AND address_street_name = "Franklin Ave";

7.
SELECT *
FROM interview
WHERE person_id IN ("14887", "16371");

8.
SELECT *
FROM get_fit_now_check_in
WHERE membership_id LIKE '48Z%'
  AND check_in_date = "20180109";

9.
SELECT *
FROM drivers_license
WHERE gender = "male"
  AND plate_number LIKE '%H42W%';

10.
SELECT *
FROM person
WHERE license_id IN ("423327", "664760");

11.
SELECT *
FROM get_fit_now_member
WHERE person_id IN ("51739", "67318");

12.
INSERT INTO solution VALUES (1, 'Jeremy Bowers');
SELECT value FROM solution;
![Screenshot 2024-09-24 123346 murdermysteryss1](https://github.com/user-attachments/assets/0c7dc0ce-4da0-4be5-9b83-a7c2485943d0)

13.
SELECT *
FROM interview
WHERE person_id = "67318";

14.
SELECT *
FROM drivers_license
WHERE gender = "female"
  AND hair_color = "red"
  AND height BETWEEN 65 AND 67
  AND car_make = "Tesla"
  AND car_model = "Model S";

15.
SELECT *
FROM person
WHERE license_id IN ("202298", "291182", "918773");

16.
SELECT 
  person_id, 
  event_name, 
  COUNT(*) AS event_count
FROM facebook_event_checkin
WHERE person_id IN ("78881", "90700", "99716")
GROUP BY person_id, event_name;

17.
INSERT INTO solution VALUES (1, 'Miranda Priestly');
SELECT value FROM solution;

![Screenshot 2024-09-24 124011 murdermysteryss2](https://github.com/user-attachments/assets/b383ab81-646f-4f8f-97f0-a6212303e2c8) 



