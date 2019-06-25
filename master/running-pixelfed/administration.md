# Administration

[[toc]]

## Admin user

> You can give a user the admin role with the command `php artisan user:admin USER`. USER can be a user id or a user name.

Optionally, you can do it manually

```
$ php artisan tinker

>>> $username = 'username_here';

>>> $user = User::whereUsername($username)->firstOrFail();

>>> $user->is_admin = true;

>>> $user->save();
```
