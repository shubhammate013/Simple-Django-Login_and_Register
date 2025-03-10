# Simple Django Login and Registration

An example of Django project with basic user functionality.

## Screenshots

| Log In | Create an account | Authorized page |
| -------|--------------|-----------------|
| <img src="source/screenshots/login.png" width="200"> | <img src="source/screenshots/create_an_account.png" width="200"> | <img src="source/screenshots/authorized_page.png " width="200"> |

| Password reset | Set new password | Password change |
| ---------------|------------------|-----------------|
| <img src="source/screenshots/password_reset.png" width="200"> | <img src="source/screenshots/set_new_password.png" width="200"> | <img src="source/screenshots/password_change.png" width="200"> |

## Functionality

- Log in
    - via username & password
    - via email & password
    - via email or username & password
    - with a remember me checkbox (optional)
- Create an account
- Log out
- Profile activation via email
- Reset password
- Remind a username
- Resend an activation code
- Change password
- Change email
- Change profile
- Multilingual: English, French, Russian, Simplified Chinese and Spanish


## Installing

### Clone the project

```bash
git clone https://github.com/shubhammate013/Simple-Django-Login_and_Register.git
cd Simple-Django-Login_and_Register
```

### Install dependencies & activate virtualenv

#### Create a virtualenv using conda (optional)

```bash
conda create -n Simple-Django-Login_and_Register python=3.11

conda activate Simple-Django-Login_and_Register
```

#### Install dependencies

```bash
pip install -U poetry

poetry install
poetry shell
```

### Configure the settings (connection to the database, connection to an SMTP server, and other options)

1. Edit `source/app/conf/development/settings.py` if you want to develop the project.

2. Edit `source/app/conf/production/settings.py` if you want to run the project in production.

### Apply migrations

```bash
python source/manage.py migrate
```

### Collect static files (only on a production server)

```bash
python source/manage.py collectstatic
```

### Running

#### A development server

Just run this command:

```bash
python source/manage.py runserver
```
