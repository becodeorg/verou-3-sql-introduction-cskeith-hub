# SQL introduction


## Must-have features

1. I did set up a database in phpMyAdmin
#
2. Create tables

    - groups: id, name, location, start_date, max_participants 
    - learners: id, name, email, active
    - coaches: id, name
#
3. selecting

    1. Get all data from the groups 
    -  SELECT * FROM `groups`;

    2. Get the name and email of the first learner, and alias the name to learner_name*
    - SELECT id, email, name AS learner_name FROM learners WHERE id = 1;
