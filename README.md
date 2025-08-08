# Exploring Java Date and Time API

## Exercise 1: LocalDate and DateTimeFormatter

**Prediction:**

* Default format will be `YYYY-MM-DD`.
* First custom format will show `DD/MM/YYYY`.
* Second format will show the full day and month name.

**Observation:**

```
Default format: 2025-08-21  
Custom format 1: 21/08/2025  
Custom format 2: Thursday, August 21, 2025
```

---

## Exercise 2: LocalTime and Formatting

**Prediction:**

* Default format will show current time in 24-hour format.
* The custom format should also work correctly for both 24-hour and 12-hour styles.

**Observation:**

```
Default format: 16:45:30  
24-hour format: 16:45:30  
12-hour format with AM/PM: 04:45:30 PM
```

---

## Exercise 3: LocalDateTime and Custom Format

**Prediction:**

* Default format will include both date and time separated by `T`.
* Custom format will show abbreviated month name and 12-hour time with AM/PM.

**Observation:**

```
Default format: 2025-11-27T19:00  
Custom format: Nov 27, 2025 at 07:00 PM
```

---

## Exercise 4: Immutability

**Prediction:**

* LocalDate is immutable, so changes result in a new object.
* Printing the original after modification should still show the original date.

**Observation:**

```
Start date after trying to modify it: 2025-09-01  
The original start date is still: 2025-09-01  
The new end date is: 2025-09-11
```

---

## Exercise 5: DateTime Arithmetic

**Prediction:**

* The base datetime will adjust forward and backward using plus/minus methods.
* `plusYears`, `plusMonths`, and `plusHours` will stack correctly.
* `minusWeeks` will move the date earlier.

**Observation:**

```
Base time:   2025-10-15 10:30  
Future time: 2026-12-15 15:30  
Past time:   2025-09-21 10:30
```

---

## Exercise 6: Period Calculation

**Prediction:**

* Using `Period.between` should return years, months, and days difference.
* Should print 2 years, 4 months, and 5 days if dates are correctly set.

**Observation:**

```
The period between the two dates is: 2 years, 4 months, and 5 days.
```


