# Deleted User List
A list of some deleted discord user ids that can be used to filter out irrelevant db entries. 
Feel free to make a pull request and add more users to the list.

Users are considered deleted when they meet one of these requirements:
- `GET /users/{user_id}` results in 404
- The discriminator is #0000
- The username matches `^Deleted User .+$` and the avatar is null

These requirements may result in some false-positives, but in that case it's the users fault imo.