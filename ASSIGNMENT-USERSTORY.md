# Congestion Tax Calculator

## The Scenario

Your colleague started working on an application for calculating congestion tax fees for vehicles within the Tehran area. Unfortunately, said colleague has gone on parental leave and left the half-finished project to you. While there are no syntax errors in the attached code, there seem to be bugs in the calculation, and there is no entry point to the project, only a class library that currently isn't called from anywhere.
Looking around your colleague's desk, you find a list of dates scribbled on a post-it. Maybe they'll come in handy.

"2013-01-14 21:00:00"

"2013-01-15 21:00:00"

"2013-02-07 06:23:27"

"2013-02-07 15:27:00"

"2013-02-08 06:27:00"

"2013-02-08 06:20:27"

"2013-02-08 14:35:00"

"2013-02-08 15:29:00"

"2013-02-08 15:47:00"

"2013-02-08 16:01:00"

"2013-02-08 16:48:00"

"2013-02-08 17:49:00"

"2013-02-08 18:29:00"

"2013-02-08 18:35:00"

"2013-03-26 14:25:00"

"2013-03-28 14:07:27"

## Assignment

**We want you to think through and implement the user stories Of an application to implement a solution that solves the problem and that you would approve and could stand for.**

Business requirements for calculating vehicle tolls are given below. Implement these requirements in the form of User Stories. 

Implemented user stories must be written based on one of the standard formats.

Implemented user stories should not violate SMART and INVEST principles.

For each User Story, you must specify the appropriate Acceptance Criteria.

## Congestion tax rules in Tehran

Congestion tax is charged during fixed hours for vehicles driving into and out of Tehran.

The maximum amount per day and vehicle is 800,000 Rials.

The tax is charged at half price on weekends (Thursdays and Fridays), public holidays, and days before a public holiday.

### Hours and amounts for congestion tax in Tehran

| Time        | Amount |
| ----------- | :----: |
| 06:00–06:29 | 100,000 Rials |
| 06:30–06:59 | 150,000 Rials |
| 07:00–07:59 | 200,000 Rials |
| 08:00–08:29 | 150,000 Rials |
| 08:30–14:59 | 100,000 Rials |
| 15:00–15:29 | 150,000 Rials |
| 15:30–16:59 | 200,000 Rials |
| 17:00–17:59 | 150,000 Rials |
| 18:00–22:29 | 100,000 Rials |
| 22:30–05:59 | 0       Rials |

### The single charge rule

A single charge rule applies in Tehran. Under this rule, a vehicle that passes several tolling stations within 60 minutes is only taxed once. The amount that must be paid is the highest one.

### Tax Exempt vehicles

- Emergency vehicles
- Busses
- Diplomat vehicles
- Taxis
- Military vehicles
- Foreign vehicles
