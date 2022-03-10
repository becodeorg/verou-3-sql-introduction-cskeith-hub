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
    #

    2. Get the name and email of the first learner, and alias the name to learner_name*

    - SELECT id, email, name AS learner_name FROM learners WHERE id = 1;
    #
4. shit happens

    1. Update the start date of the first_group (make it two months later)

    -  UPDATE groups SET start_date = '2022-02-14' WHERE Id = 1 
    #
    2. Introduce a new field `status` which can contain a long text indicating the reason for postponing (bonus points if it's a creative one)

    - ALTER TABLE groups ADD  status_group TEXT AFTER max_participants;
    #
5. Delete someone from the learners table

    - DELETE FROM learners WHERE id = 1;
