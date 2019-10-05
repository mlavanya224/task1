# task1

## step1
create database (task1) and execute query

CREATE TABLE IF NOT EXISTS `users` (
  `user_id` int(11) NOT NULL AUTO_INCREMENT,
  `username` varchar(60) NOT NULL,
  `password` varchar(255) NOT NULL,
  `first_name` varchar(40) NOT NULL,
  `last_name` varchar(55) NOT NULL,
  `profile_image` varchar(255) NOT NULL,
   PRIMARY KEY (`user_id`)
); 
CREATE TABLE IF NOT EXISTS `posts` (
  `post_id` int(11) NOT NULL AUTO_INCREMENT,
  `user_id_p` int(11) NOT NULL,
  `status` text NOT NULL,
  `status_image` varchar(255) NOT NULL,
  `status_time` timestamp NOT NULL DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP,
  PRIMARY KEY (`post_id`)
);

## step2
 php code download and execute
