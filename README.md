# Twiiter Database Sample Data

This repository contains sample data for a Database with three users: Vader, Leia, and Obi-Wan. The data includes user information, tweets, likes, followers, and retweets to demonstrate the relationships within the system.

## Tables

### Users

| id | email                | password             | name    | phone_number  | followers_count | following_count | tweet_count |
|----|----------------------|----------------------|---------|---------------|-----------------|------------------|-------------|
| 1  | Vader1@gmail.com     | Vaderpassword@1      | Vader   | 1234567890    | NULL            | NULL             | NULL        |
| 2  | Leia0@gmail.com      | Leiapassword@2       | Leia    | 987654321     | NULL            | NULL             | NULL        |
| 3  | wan3@gmail.com       | Obi-Wanpassword@3    | Obi-Wan | 7798347983   | NULL            | NULL             | NULL        |

### Likes

| likeId | tweetId | userId | created_at         |
|--------|---------|--------|---------------------|
| 1      | NULL    | 2      | 2024-01-25 15:40:45 |

### Tweets

| tweetId | userId | tweetContent                            | created_at         |
|---------|--------|-----------------------------------------|---------------------|
| 1       | 1      | I find your lack of faith disturbing.   | 2024-01-25 15:30:45 |
| 2       | 3      | The Force will be with you. Always.      | 2024-01-25 15:35:00 |
| 3       | 2      | Help me, Obi-Wan Kenobi. You're my only hope. | 2024-01-25 15:35:00 |

### Followers

| id | followerId | followingId | created_at         |
|----|------------|-------------|---------------------|
| 1  | 2          | 1           | 2024-01-25 16:10:45 |
| 2  | 1          | 3           | 2024-01-25 16:20:45 |

### Retweets

| retweetId | tweetId | userId | created_at         |
|-----------|---------|--------|---------------------|
| 1         | 1       | 3      | 2024-01-25 16:30:45 |

## Sample Relationships

- Leia likes Vader's tweet.
- Obi-Wan retweets Vader's tweet.
- Leia follows Vader, and Vader follows Obi-Wan.

This sample data demonstrates the relationships and interactions between the users in the Twitter.

