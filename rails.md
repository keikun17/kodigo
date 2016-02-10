Rails
-----

Generate secret key :

    rake secret

    // or

    rails secret

Rollback migration

    rails db:rollback
    // or specify number of steps for undoing several migrations
    rails db:rollback STEP=3

Redo migrations (rollback then migrate up)

    rails db:migrate:redo
    // or specify number of steps for redoing several migrations
    rails db:migrate:redo STEP=4
