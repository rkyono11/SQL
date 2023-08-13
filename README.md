# Shelly Kyono's SQL Portfolio
**Hello and welcome to my SQL Portfolio! This code repository represents examples of SQL I've written.
Feel free to check it out and contact me through email if you have any questions:**

CREATE TABLE mystical_crafts (id INTEGER PRIMARY KEY, item TEXT, ordered INTEGER, price INTEGER, purchased INTEGER, returned INTEGER, write_off INTEGER);

INSERT INTO mystical_crafts VALUES (1, "Rose Quarts Minis", 150, 7.00, 24, 6, 9); 
INSERT INTO mystical_crafts VALUES (2, "3 Pack Incense Cones", 200,  2.50, 48, 0, 5);
INSERT INTO mystical_crafts VALUES (3, "Palo Santo Wood", 200, 3.00, 55, 2, 9);
INSERT INTO mystical_crafts VALUES (4, "2 Pack Stick Incense", 400, 1.00, 320, 50, 10);
INSERT INTO mystical_crafts VALUES (5, "White Tea Candles", 500, .50, 500, 0, 0);
INSERT INTO mystical_crafts VALUES (6, "5 Pack Taper Candles", 100, 4.00, 49, 7, 7);
INSERT INTO mystical_crafts VALUES (7, "Frankincense Resin", 80, 5.00, 28, 0, 1);
INSERT INTO mystical_crafts VALUES (8, "Long Ritual Matches", 70, 5.50, 20, 1, 0);
INSERT INTO mystical_crafts VALUES (9, "Raw Selenite", 150, 9.50, 99, 0, 2);
INSERT INTO mystical_crafts VALUES (10, "Amethyst Points", 85, 12.50, 79, 3, 0);
INSERT INTO mystical_crafts VALUES (11, "Bath Salts", 50, 15.00, 30, 9, 2);
INSERT INTO mystical_crafts VALUES (12, "Witchcraft for Beginners Booklet", 40, 12.00, 40, 0, 0);
INSERT INTO mystical_crafts VALUES (13, "Wild Rosemary Smudge Stick", 60, 6.00, 30, 0, 3);
INSERT INTO mystical_crafts VALUES (14, "Witches Black Salt", 40, 5.00, 10, 0, 0);
INSERT INTO mystical_crafts VALUES (15, "Selenite Towers", 5, 100.00, 2, 0, 0);


SELECT item, price FROM mystical_crafts ORDER BY price;

SELECT item, ordered, SUM(purchased) FROM mystical_crafts GROUP BY purchased ORDER BY item;
