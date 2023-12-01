# Learning Simple Laravel 10

#### Project Idea
1. User can create a new help ticket
2. Admin can reply on help ticket
3. Admin can reject or resolve the ticket
4. When admin update on the ticket the user will get on notif via email
5. User can give ticket title and desc
6. User can upload document

#### Table
1. Tickets
    - title(string){required}
    - description(text){required}
    - status(open{default},resolved,rejected)
    - attachment(string) {nullabel}
    - user_id {required}
    - status_changed_by_id {nullable}

2. Replies
    - body(text){required}
    - user_id {required} filled by laravel
    - ticket_id {required} filled by laravel