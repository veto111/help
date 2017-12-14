
Items for sale table:
CREATE TABLE `items_for_sale` (
 `id` int(11) NOT NULL AUTO_INCREMENT,
 `item_name` varchar(250) NOT NULL,
 `item_price` decimal(8,2) NOT NULL,
 `image_addr` varchar(500) NOT NULL,
 `created_at` timestamp NOT NULL DEFAULT CURRENT_TIMESTAMP,
 PRIMARY KEY (`id`),
 UNIQUE KEY `item_name` (`item_name`)
) ENGINE=InnoDB AUTO_INCREMENT=13 DEFAULT CHARSET=latin1

Orders table:
CREATE TABLE `orders` (
 `id` int(11) NOT NULL AUTO_INCREMENT,
 `chargeId` varchar(250) NOT NULL,
 `clientId` varchar(11) NOT NULL,
 `description` text NOT NULL,
 `charge_amount` decimal(10,2) NOT NULL,
 `created_at` timestamp NOT NULL DEFAULT CURRENT_TIMESTAMP,
 PRIMARY KEY (`id`)
) ENGINE=InnoDB AUTO_INCREMENT=2 DEFAULT CHARSET=latin1

Users table:
CREATE TABLE `users` (
 `id` int(11) NOT NULL AUTO_INCREMENT,
 `name` varchar(30) NOT NULL,
 `username` varchar(30) NOT NULL,
 `password` varchar(255) NOT NULL,
 `email` varchar(30) NOT NULL,
 `created_at` timestamp NOT NULL DEFAULT CURRENT_TIMESTAMP,
 PRIMARY KEY (`id`)
) ENGINE=InnoDB AUTO_INCREMENT=15 DEFAULT CHARSET=latin1
