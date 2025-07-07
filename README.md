# README

(users table)
- id:integer
- email:string [present]
- encrypted_password:string
- reset_password_token:string
- remember_password_sent_at:datetime
- remember_created_at:datetime
- created_at:datetime
- updated_at:datetime
- has_many posts

(posts table)
- id:integer
- title:string [present, unique, 4-50 chars]
- body:text [present]
- created_at:datetime
- updated_at:datetime
- belongs_to user
- user_id:integer [present, foreign key]

