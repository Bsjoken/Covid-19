SELECT *
FROM `bustling-winter-371116.Covid_19.Covid`
ORDER BY 3, 4

-Selecting the data we are going to be using

SELECT SEX, PREGNANT, AGE, DIABETES, PNEUMONIA
FROM `bustling-winter-371116.Covid_19.Covid`
WHERE PATIENT_TYPE IS NOT NULL

-Looking at cases where people were pregnat that had diabetes between the ages of 20-40 years old

SELECT PREGNANT, DIABETES, AGE
FROM `bustling-winter-371116.Covid_19.Covid`
WHERE AGE BETWEEN 20 AND 40

-Looking at cases of when people died between ages 10-30 years old

SELECT DATE_DIED
FROM `bustling-winter-371116.Covid_19.Covid`
WHERE AGE BETWEEN 10 and 30

-Looking to see which sex had the most cases with diabetes

SELECT SEX, DIABETES
FROM `bustling-winter-371116.Covid_19.Covid`
WHERE SEX = 1

SELECT SEX, DIABETES
FROM `bustling-winter-371116.Covid_19.Covid`
WHERE SEX = 2
