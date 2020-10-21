# Go LINE
LINE clone using go

## Fitur
- Register
- Login
- Add Friend
- Chat between user
- Chat in group
- Posting timeline
- Edit post in timeline
- Delete post in timeline
- Get all post in timeline
- Edit profile
- Get profile
- Call

## Schema
1. User
    - Uid: String(16); Primary Key
    - fullName: String
    - userName: String; Unique
    - password: String
    - email: String
    - photoProfile: String/GLOB; Nullable
    - status: String; Nullable
2. Post
    - Uid: String(16); Primary Key
    - image: String; Nullable
    - caption: String
    - Author: String(16)
    - type: enum("g", "t") # Indicator for group post and timeline post
3. Group
    - Uid: String(16); Primary Key
    - member: String; # Uid Member
    - photoProfile: String 
4. Chat
    - from: String(16)
    - to: String(16)
    - content: String

## Progress
* :white_check_mark: Init project
